---
title: fileEncryptionInfo リソースの種類
description: ビジネス アプリの行のコンテンツ バージョンのファイル暗号化情報のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f9d9dce2516c1978058dd1c9ddbf2211a3d88da
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620256"
---
# <a name="fileencryptioninfo-resource-type"></a>fileEncryptionInfo リソースの種類

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ビジネス アプリの行のコンテンツ バージョンのファイル暗号化情報のプロパティが含まれています。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|encryptionKey|Binary|ファイルのコンテンツを暗号化するために使用するキーです。|
|initializationVector|Binary|暗号化アルゴリズムに使用される初期化ベクトルです。|
|Mac|Binary|暗号化されたファイル コンテンツのハッシュ + IV (コンテンツ ハッシュ) です。|
|macKey|Binary|Mac を取得するために使用するキーです。|
|profileIdentifier|String|プロファイル識別子。|
|fileDigest|Binary|暗号化される前のファイル ダイジェストです。|
|fileDigestAlgorithm|String|ファイル ダイジェストのアルゴリズムです。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fileEncryptionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fileEncryptionInfo",
  "encryptionKey": "binary",
  "initializationVector": "binary",
  "mac": "binary",
  "macKey": "binary",
  "profileIdentifier": "String",
  "fileDigest": "binary",
  "fileDigestAlgorithm": "String"
}
```



