# <a name="grouplifecyclepolicy-resource-type"></a>groupLifecyclePolicy リソース タイプ

Office 365 グループのライフサイクル ポリシーを表します。 グループのライフサイクル ポリシーにより、管理者はグループに対して有効期限を設定できます。 たとえば、180 日後にグループの有効期限が切れます。 グループの有効期限に達すると、グループの所有者は、管理者が定義した時間間隔内でグループを更新する必要があります。 更新されると、グループの有効期限はポリシーで定義された日数、延長されます。 たとえば、グループの新しい有効期限は、更新後 180 日です。 グループが更新されない場合、グループの有効期限が切れ、削除されます。 グループは、削除から 30 日以内に復元できます。

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:---------------|:--------|:----------|
|[Get groupLifecyclePolicy](../api/grouplifecyclepolicy_get.md) | [groupLifecyclePolicy](grouplifecyclepolicy.md) |groupLifecyclePolicy オブジェクトのプロパティとリレーションシップを読み取ります。|
|[List groupLifecyclePolicies](../api/grouplifecyclepolicy_list.md) | [groupLifecyclePolicy](grouplifecyclepolicy.md) コレクション | すべての groupLifecyclePolicies を一覧表示します。 |
|[Update groupLifecyclePolicy](../api/grouplifecyclepolicy_update.md) | [groupLifecyclePolicy](grouplifecyclepolicy.md) | groupLifecyclePolicy を更新します。 |
|[Delete groupLifecyclePolicy](../api/grouplifecyclepolicy_delete.md) | なし | groupLifecyclePolicy オブジェクトを削除します。 |
|[Add a group to a groupLifecyclePolicy](../api/grouplifecyclepolicy_addgroup.md)|なし| ライフ サイクル ポリシーにグループを追加します。 |
|[Remove a group from a groupLifecyclePolicy](../api/grouplifecyclepolicy_removegroup.md)|なし| ライフ サイクル ポリシーからグループを削除します。 |

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|alternateNotificationEmails|String| 所有者のいないグループに対して通知を送信する電子メール アドレスのリスト 電子メール アドレスをセミコロンで区切って、複数の電子メール アドレスを定義することができます。 |
|groupLifetimeInDays|Int32| グループの有効期限が切れ、更新が必要になるまでの日数。 更新されると、グループの有効期限は定義された日数、延長されます。 |
|ID|Guid| ポリシーの一意の識別子。 読み取り専用です。|
|managedGroupTypes|String| 有効期限ポリシーを適用するグループの種類。 可能な値は、**All**、**Selected**、または **None** です。 |

## <a name="relationships"></a>リレーションシップ

なし。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
}-->

```json
{
  "alternateNotificationEmails": "String",
  "groupLifetimeInDays": 180,
  "id": "Guid (identifier)",
  "managedGroupTypes": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->