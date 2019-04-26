---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
localization_priority: Normal
ms.openlocfilehash: abe6fc277f94eb1f66f50f25b894bc41fd038a9b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570821"
---
# <a name="hashes-resource-type"></a>Hashes リソース型

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
| **crc32Hash**    | String | リトルエンディアン内のファイルの CRC32 値 (使用可能な場合)。 読み取り専用。            |
| **quickXorHash** | String | ファイルの内容が変更されているかどうかの判別に使用できるファイルの専用ハッシュ (使用可能な場合)。読み取り専用。 |

**注:** ハッシュ値が使用可能ではない場合があります。その場合、アイテムのハッシュ値は、アイテムがダウンロードされた後に更新されます。

## <a name="remarks"></a>備考

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
