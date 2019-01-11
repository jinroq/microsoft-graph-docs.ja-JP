---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: RemoteItem
localization_priority: Normal
ms.openlocfilehash: 0b29ba14273bad7306518c290029a9ebc444f07d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888089"
---
# <a name="remoteitem-resource-type"></a>RemoteItem リソースの種類

**remoteItem** リソースは、[**driveItem**](driveitem.md) が別のドライブに存在するアイテムを参照することを示します。このリソースは、ソース ドライブとターゲット項目の固有 ID を提供します。

非 null の **remoteItem** ファセットを持つ [**DriveItems**](driveitem.md)は、共有された、ユーザーの OneDrive に追加された、あるいは異質な項目のコレクション (検索結果など) から返される項目上にあるリソースです。

**注:** 同じドライブにあるフォルダーとは異なり、リモート アイテムに移動された **driveItem** では、`id` 値が変更された可能性があります。

## <a name="json-representation"></a>JSON 表記

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.remoteItem", 
       "optionalProperties": ["name", "fileSystemInfo", "file", "folder"] } -->

```json
{
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "file": { "@odata.type": "microsoft.graph.file" },
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "folder": { "@odata.type": "microsoft.graph.folder" },
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "name": "string",
  "package": { "@odata.type": "microsoft.graph.package" },
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "shared": { "@odata.type": "microsoft.graph.shared" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "specialFolder": { "@odata.type": "microsoft.graph.specialFolder" },
  "size": 1024,
  "webDavUrl": "url",
  "webUrl": "url"
}
```

## <a name="properties"></a>プロパティ

| プロパティ名        | 種類                                | 説明                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| createdBy            | [IdentitySet](identityset.md)       | その項目を作成したユーザー、デバイス、およびアプリケーションの ID。読み取り専用。                                                                                  |
| createdDateTime      | Timestamp                           | 項目作成の日付と時刻。読み取り専用。                                                                                                                        |
| file                 | [File](file.md)                     | リモート項目がファイルであることを示します。読み取り専用。                                                                                                              |
| fileSystemInfo       | [FileSystemInfo](filesysteminfo.md) | ローカル ファイル システムからのリモート項目についての情報。読み取り専用。                                                                                          |
| folder               | [Folder](folder.md)                 | リモート項目がフォルダーであることを示します。読み取り専用。                                                                                                            |
| id                   | String                              | ドライブ内のリモート項目の固有識別子です。読み取り専用。                                                                                                    |
| lastModifiedBy       | [IdentitySet](identityset.md)       | 最後にその項目を修正したユーザー、デバイス、およびアプリケーションの ID。読み取り専用。                                                                            |
| lastModifiedDateTime | Timestamp                           | アイテムが最後に変更された日時。読み取り専用。                                                                                                              |
| name                 | String                              | 省略可能。リモート項目のファイル名です。読み取り専用。                                                                                                                 |
| package              | [Package](package.md)               | 存在する場合、この項目がフォルダーやファイルではなくパッケージであることを示します。パッケージは、一部のコンテキストでのファイルのように、他のコンテキストではフォルダーのように扱われます。読み取り専用。 |
| parentReference      | [ItemReference](itemreference.md)   | リモート項目の親のプロパティです。読み取り専用です。                                                                                                           |
| shared               | [shared](shared.md)                 | アイテムが他のユーザーと共有されていることを示し、アイテムの共有状態に関する情報を提供します。読み取り専用です。                                       |
| sharepointIds        | [SharepointIds](sharepointids.md)   | OneDrive for Business と SharePoint 間の相互運用を、項目識別子の完全なセットと共に提供します。読み取り専用。                                          |
| size                 | Int64                               | リモート項目のサイズです。読み取り専用です。                                                                                                                               |
| specialFolder        | [specialFolder][]                   | 現在のアイテムが特別なフォルダーとしても使用可能な場合は、このファセットが返されます。読み取り専用です。                                                                     |
| webDavUrl            | Url                                 | 項目の、DAV 互換性のある URL です。                                                                                                                                  |
| webUrl               | Url                                 | ブラウザーでリソースを表示するための URL。読み取り専用。                                                                                                         |

[specialFolder]: specialfolder.md

## <a name="remarks"></a>備考

**driveItem** のファセットに関する詳細については、「[driveItem](driveitem.md)」を参照してください。

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem"
} -->
