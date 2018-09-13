# <a name="update-alert"></a>警告の更新

統合ソリューション内の編集可能な**警告**プロパティを更新して、 ソリューション間で警告の状態と割り当ての同期を維持します。 このメソッドは、参照されている警告 ID のレコードのあるすべてのソリューションを更新します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校アカウント) |   SecurityEvents.ReadWrite.All  |
|委任 (個人用 Microsoft アカウント) |  サポートされていません。  |
|アプリケーション | SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

> **注:** このメソッドでは、`provider` と `vendor` を含むパラメーターと vendorInformation として、**警告** ID を含める必要があります。
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 説明|
|:-----------|:-----------|
| 承認  | Bearer {code}。必須。|
|優先 | 返す = 表現 |

## <a name="request-body"></a>要求本文

要求本文で、更新する関連フィールドの値の JSON 表記を指定します。 本文には、有効な`provider` と `vendor`フィールドのある `vendorInformation` プロパティが含まれて**いなければなりません**。 次の表では、警告の更新可能なフィールドを示します。 要求の本文に含まれない既存のプロパティの値は変更されません。 最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。

| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
|assignedTo|文字列|警告は、アナリストの名前を選別、調査、または修復に割り当てます。|
|closedDateTime|DateTimeOffset|警告が終了した時間。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 |||UNTRANSLATED_CONTENT_START|||For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.|||UNTRANSLATED_CONTENT_END||||
|コメント|String コレクション|警告 (顧客の警告管理用) に関するアナリストのコメントです。|
|フィードバック|alertFeedback|警告に関するアナリストのフィードバックです。 可能な値は、`unknown`、`truePositive`、`falsePositive`、`benignPositive` です。|
|状態|alertStatus|アラートのライフ サイクル ステータス (ステージ)。 可能な値は、`unknown`、`newAlert`、`inProgress`、`resolved` です。|
|タグ|String コレクション|警告に適用でき、フィルター条件 ("HVA"、"SAW" など) として機能できるユーザーが定義可能なラベル。|
|vendorInformation *|[securityVendorInformation](../resources/securityvendorinformation.md)|セキュリティ製品、またはサービスの仕入先、サービス プロバイダー、およびサービス サブプロバイダーの詳細を含む複合型 (仕入先 = Microsoft、プロバイダー = Windows Defender ATP、サブプロバイダー = AppLocker など)。 **プロバイダーおよび仕入先のフィールドは必須です。**|
(\* は、必須フィールドを表します)。

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。

オプションの要求ヘッダーが使われている場合、このメソッドは`200 OK`応答コードと、応答本文で[警告](../resources/alert.md)オブジェクトを返します。

## <a name="example-1"></a>例 1

### <a name="request"></a>要求

要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
Content-type: application/json

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```

### <a name="response"></a>応答

正常な応答の例を次に示します。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="example-2"></a>例 2

### <a name="request"></a>要求

次の例では、`Prefer` 要求ヘッダーを含む要求を示します。

<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
Content-type: application/json
Prefer: return=representation

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```

### <a name="response"></a>応答

|||UNTRANSLATED_CONTENT_START|||The following is an example of the response when the optional `Prefer: return=representation` request header is used.|||UNTRANSLATED_CONTENT_END|||

>**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "activityGroupName": "activityGroupName-value",
  "assignedTo": "assignedTo-value",
  "azureSubscriptionId": "azureSubscriptionId-value",
  "azureTenantId": "azureTenantId-value",
  "category": "category-value",
  "closedDateTime": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update alert",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
