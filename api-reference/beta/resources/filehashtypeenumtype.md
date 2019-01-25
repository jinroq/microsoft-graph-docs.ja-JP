---
title: fileHashType 列挙型
description: ファイル ハッシュの種類を列挙します。
localization_priority: Normal
ms.openlocfilehash: 082fdd9cdad6c3ec1ea4e07020983ac0bac7ed65
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518381"
---
# <a name="filehashtype-enum"></a>fileHashType 列挙型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ファイル ハッシュの種類を列挙します。

## <a name="members"></a>メンバー

|メンバー|値|説明|
|:---|:---|:---|
|不明|(0)|不明な種類です。|
|sha1|-1|SHA1 ハッシュ タイプを入力します。|
|SHA256|-2| SHA256 ハッシュ タイプを入力します。|
|MD5|-3| MD5 ハッシュ タイプを入力します。|
|authenticodeHash256|-4| AuthenticodeHash256 ハッシュ タイプを入力します。|
|lsHash|0.5| LsHash ハッシュ タイプを入力します。|
|ctph|-6| CTPH ハッシュ タイプを入力します。|
|peSha1|-7| PESHA1 ハッシュ タイプを入力します。|
|peSha256|-8| PESHA256 ハッシュ タイプを入力します。|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/filehashtypeenumtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
