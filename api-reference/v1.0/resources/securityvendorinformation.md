# <a name="securityvendorinformation-resource-type"></a>securityVendorInformation リソースの種類

セキュリティ製品、またはサービスの仕入先、サービス プロバイダー、およびサービス サブプロバイダーの詳細を含む複合型 (仕入先 = Microsoft、プロバイダー = Windows Defender ATP、サブプロバイダー = AppLocker など)。

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|プロバイダ|文字列|特定のプロバイダー (製品やサービスの仕入先会社ではありません)。例えば、WindowsDefenderATP です。|
|providerVersion|文字列|Subprovider、それが存在する場合は、アラートを生成したプロバイダーのバージョンです。|
|subProvider|文字列|特定の subprovider 下にあるプロバイダーを集約)。例えば、WindowsDefenderATP.SmartScreen です。|
|仕入先＊|文字列|アラート ベンダー (Microsoft、Dell 、 FireEye など) の名前。|
(\* は、必須記入欄を表示します)。

## <a name="json-representation"></a>JSON 表記

次は、リソースの JSON 表現です。
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityVendorInformation"
}-->

```json
{
  "provider": "String",
  "providerVersion": "String",
  "subProvider": "String",
  "vendor": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
