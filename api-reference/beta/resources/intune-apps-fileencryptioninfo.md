---
title: fileEncryptionInfo リソースの種類
description: ビジネス アプリの行のコンテンツ バージョンのファイル暗号化情報のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9a2236e2c63703ea5af2662d5b0f4594e7888799
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552178"
---
# <a name="fileencryptioninfo-resource-type"></a>fileEncryptionInfo リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ビジネス アプリの行のコンテンツ バージョンのファイル暗号化情報のプロパティが含まれています。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|encryptionKey|Binary|ファイルのコンテンツを暗号化するために使用するキーです。|
|initializationVector|Binary|暗号化アルゴリズムに使用される初期化ベクトルです。|
|Mac|Binary|暗号化されたファイル コンテンツのハッシュ + IV (コンテンツ ハッシュ) です。|
|macKey|Binary|Mac を取得するために使用するキーです。|
|profileIdentifier|String|プロファイルの識別子です。|
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





