# <a name="mediacontentratingnewzealand-resource-type"></a>mediaContentRatingNewZealand リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません
## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|movieRating|[ratingNewZealandMoviesType](../resources/intune_deviceconfig_ratingnewzealandmoviestype.md)|評価のニュージーランドを選択したムービーです。使用可能な値: `allAllowed`、 `allBlocked`、 `general`、 `parentalGuidance`、 `mature`、 `agesAbove13`、 `agesAbove15`、 `agesAbove16`、 `agesAbove18`、 `restricted`、 `agesAbove16Restricted`。|
|tvRating|[ratingNewZealandTelevisionType](../resources/intune_deviceconfig_ratingnewzealandtelevisiontype.md)|ニュージーランド向けに選択されているテレビのレーティング。可能な値: `allAllowed` 、`allBlocked` 、`general` 、`parentalGuidance` 、`adults` 。|

## <a name="relationships"></a>関係
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```








