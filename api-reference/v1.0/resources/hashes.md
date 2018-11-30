---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
ms.openlocfilehash: 92882910ecf86d19e1f0a8a5767d148f5aa95775
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023644"
---
# <a name="hashes-resource-type"></a>ハッシュ リソースの種類

 **ハッシュ** リソースは、利用可能なハッシュをアイテムの 1 つの構造にグループ化します。

**注:** すべてのサービスで、表示されているすべてのハッシュ プロパティに対して値が指定されているわけではありません。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "sha1Hash", "crc32Hash", "quickXorHash" ],
  "@odata.type": "microsoft.graph.hashes"
}-->

```json
{
  "crc32Hash": "string (hex)",
  "sha1Hash": "string (hex)",
  "quickXorHash": "string (base64)"
}
```

## <a name="properties"></a>プロパティ

| プロパティ         | 型   | 説明                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| **sha1Hash**     | String | ファイルの内容の SHA1 ハッシュ (使用可能な場合)。読み取り専用。 |
| **crc32Hash**    | String | リトルエンディアン (ある場合) 内のファイルの CRC32 の値です。 読み取り専用。            |
| **quickXorHash** | String | ファイルの内容が変更されているかどうかの判別に使用できるファイルの専用ハッシュ (使用可能な場合)。読み取り専用。 |

**注:** ハッシュ値が使用可能ではない場合があります。その場合、アイテムのハッシュ値は、アイテムがダウンロードされた後に更新されます。

## <a name="remarks"></a>注釈

OneDrive for Business および SharePoint Server 2016 では、**sha1Hash** と **crc32Hash** は利用できません。

OneDrive 個人用では、**quickXorHash** は利用できません。

ファイルに対する **quickXorHash** を計算する場合は、[QuickXorHash スニペット](https://dev.onedrive.com/snippets/quickxorhash.htm)を参照してください。
DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。


<!-- {
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes"
} -->
