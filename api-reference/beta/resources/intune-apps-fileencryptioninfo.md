---
title: fileEncryptionInfo リソースの種類
description: ビジネス アプリの行のコンテンツ バージョンのファイル暗号化情報のプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3a507aed30d82fd012a964082a2d83fed0f7c751
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950425"
---
# <a name="fileencryptioninfo-resource-type"></a>fileEncryptionInfo リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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

## <a name="relationships"></a>関係
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




