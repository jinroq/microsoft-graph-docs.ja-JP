# <a name="mediacontentratingnewzealand-resource-type"></a>mediaContentRatingNewZealand リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません
## <a name="properties"></a>プロパティ
|プロパティ|タイプ|説明|
|:---|:---|:---|
|movieRating|[ratingNewZealandMoviesType](../resources/intune_deviceconfig_ratingnewzealandmoviestype.md)|ニュージーランド向けに選択された映画の評価です。 指定できる値は、`allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted` です。|
|tvRating|[ratingNewZealandTelevisionType](../resources/intune_deviceconfig_ratingnewzealandtelevisiontype.md)|ニュージーランド向けに選択されたテレビの評価です。 指定できる値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults`です。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```



