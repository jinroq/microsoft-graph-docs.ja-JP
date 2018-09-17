# <a name="mediacontentratingunitedstates-resource-type"></a>mediaContentRatingUnitedStates リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません
## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|movieRating|[ratingUnitedStatesMoviesType](../resources/intune_deviceconfig_ratingunitedstatesmoviestype.md)|評価の米国の選択したムービーです。使用可能な値: `allAllowed`、 `allBlocked`、 `general`、 `parentalGuidance`、 `parentalGuidance13`、 `restricted`、 `adults`。|
|tvRating|[ratingUnitedStatesTelevisionType](../resources/intune_deviceconfig_ratingunitedstatestelevisiontype.md)|テレビの視聴制限はアメリカ合衆国を選択します。使用可能な値: `allAllowed`、 `allBlocked`、 `childrenAll`、 `childrenAbove7`、 `general`、 `parentalGuidance`、 `childrenAbove14`、 `adults`。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```








