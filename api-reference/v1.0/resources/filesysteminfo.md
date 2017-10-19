---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FileSystemInfo
ms.openlocfilehash: 9a5214f9c5e161de0be66ac634c7c5538b203772
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="filesysteminfo-facet"></a>FileSystemInfo ファセット

**FileSystemInfo** リソースには、アイテムのローカル バージョンについてデバイスのローカル ファイル システムによって報告されるプロパティが含まれています。
このファセットは、ローカル デバイス上でアイテムが最後に更新された日付または作成された日付を指定するために使用できます。

これは、[driveItem][item-resource] リソースの fileSystemInfo プロパティで使用できます。

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "lastAccessedDateTime"
  ],
  "@odata.type": "microsoft.graph.fileSystemInfo"
}-->

```json
{
  "createdDateTime" : "datetime",
  "lastAccessedDateTime": "datetime",
  "lastModifiedDateTime" : "datetime"
}
```

## <a name="properties"></a>プロパティ

| プロパティ                 | 型           | 説明                                                                                                          |
| :----------------------- | :------------- | :------------------------------------------------------------------------------------------------------------------- |
| **createdDateTime**      | DateTimeOffset | クライアントでのファイルの作成日時 (UTC)。                                                              |
| **lastAccessedDateTime** | DateTimeOffset | ファイルに最後にアクセスした日時 (UTC)。 [最近使用したファイル一覧](../api/drive_recent.md)でのみ使用可能です。 |
| **lastModifiedDateTime** | DateTimeOffset | クライアントでファイルを最後に変更した日時 (UTC)。                                                        |

## <a name="notes"></a>メモ

**createdDateTime** と **lastModifiedDateTime** の値は、[DriveItem](driveitem.md) リソースの同じプロパティとは異なります。
DriveItem リソースの値は、サービスにより認識された作成日時と更新日時です。
**FileSystemInfo** リソースに格納される値は、クライアントから提供されます。

たとえば、あるファイルはデバイス上で月曜日に作成されたものの、火曜日までサービスにアップロードされなかった場合、ファイルをアップロードするクライアントは、`fileSystemInfo` ファセットに作成日である月曜日が含まれるように書き込む必要があります。 アイテムのメタデータを取得すると、アイテムの作成日は火曜日であると表示されますが、`fileSystemInfo` ファセットには元の作成日である月曜日が表示されます。

これらのプロパティは編集可能です。ファイルをアップロードして、これらのフィールドのローカル クライアントを知っている場合は、その値を要求に含める必要があります。

ファイルの内容を更新し、これらのプロパティが指定されていない場合、**lastModifiedDateTime** は自動的に現在の時刻にリセットされます。

## <a name="remarks"></a>備考

* **lastAccessedDateTime** は、SharePoint Online または OneDrive for Business のアイテムでは使用できません。

DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The fileSystemInfo facet provides information about date created and modified by clients.",
  "keywords": "fileSystemInfo,client,system info,onedrive",
  "section": "documentation",
  "tocPath": "Facets/FileSystemInfo"
} -->
