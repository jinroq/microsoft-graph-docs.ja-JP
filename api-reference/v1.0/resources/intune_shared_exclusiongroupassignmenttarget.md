# <a name="exclusiongroupassignmenttarget-resource-type"></a>exclusionGroupAssignmentTarget リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

割り当てから除外するグループを表します。

[groupAssignmentTarget](../resources/intune_shared_groupassignmenttarget.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|groupId|文字列|割り当てのターゲットとなるグループ ID です。 [groupAssignmentTarget](../resources/intune_shared_groupassignmenttarget.md) からの継承|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "groupId": "String"
}
```








