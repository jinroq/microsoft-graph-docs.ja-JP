---
title: mailSearchFolder リソースの種類
description: MailSearchFolder は、指定した検索条件に一致するすべてのメール アイテムが含まれているユーザーのメールボックス内の仮想フォルダーです。 mailSearchFolder は、mailFolder から継承します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ba76029b69d91be39c9d63ca755e8a4603aec0b9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520985"
---
# <a name="mailsearchfolder-resource-type"></a><span data-ttu-id="14ed4-104">mailSearchFolder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="14ed4-104">mailSearchFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14ed4-105">MailSearchFolder は、指定した検索条件に一致するすべてのメール アイテムが含まれているユーザーのメールボックス内の仮想フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="14ed4-105">A mailSearchFolder is a virtual folder in the user's mailbox that contains all the email items matching specified search criteria.</span></span> <span data-ttu-id="14ed4-106">mailSearchFolder は、 [mailFolder](mailfolder.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="14ed4-106">mailSearchFolder inherits from [mailFolder](mailfolder.md).</span></span>

## <a name="methods"></a><span data-ttu-id="14ed4-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="14ed4-107">Methods</span></span>

| <span data-ttu-id="14ed4-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="14ed4-108">Method</span></span> | <span data-ttu-id="14ed4-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="14ed4-109">Return Type</span></span>  | <span data-ttu-id="14ed4-110">説明</span><span class="sxs-lookup"><span data-stu-id="14ed4-110">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="14ed4-111">検索フォルダーを作成する</span><span class="sxs-lookup"><span data-stu-id="14ed4-111">[Create a search folder](../api/mailsearchfolder-post.md)</span></span> | [<span data-ttu-id="14ed4-112">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="14ed4-112">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="14ed4-113">このユーザーのメールボックスで検索フォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="14ed4-113">Create a search folder in this user's mailbox.</span></span> |
| [<span data-ttu-id="14ed4-114">検索フォルダーの一覧</span><span class="sxs-lookup"><span data-stu-id="14ed4-114">List search folders</span></span>](../api/mailfolder-list-childfolders.md) | <span data-ttu-id="14ed4-115">[mailFolder](mailfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="14ed4-115">[mailFolder](mailfolder.md) collection</span></span> | <span data-ttu-id="14ed4-116">検索フォルダーを含む、このユーザーのメールボックス内のすべてのフォルダーを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="14ed4-116">List all the folders in this user's mailbox, including search folders.</span></span> |
| <span data-ttu-id="14ed4-117">検索フォルダ―を取得する</span><span class="sxs-lookup"><span data-stu-id="14ed4-117">[Get a search folder](../api/mailfolder-get.md)</span></span> | [<span data-ttu-id="14ed4-118">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="14ed4-118">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="14ed4-119">指定した検索フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="14ed4-119">Get the specified search folder.</span></span> |
| <span data-ttu-id="14ed4-120">検索フォルダーを更新する</span><span class="sxs-lookup"><span data-stu-id="14ed4-120">[Update a search folder](../api/mailsearchfolder-update.md)</span></span> | [<span data-ttu-id="14ed4-121">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="14ed4-121">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="14ed4-122">指定した検索フォルダーを更新します。</span><span class="sxs-lookup"><span data-stu-id="14ed4-122">Update the specified search folder.</span></span> |
| <span data-ttu-id="14ed4-123">検索フォルダーを削除する</span><span class="sxs-lookup"><span data-stu-id="14ed4-123">[Delete a search folder](../api/mailfolder-delete.md)</span></span> | <span data-ttu-id="14ed4-124">なし</span><span class="sxs-lookup"><span data-stu-id="14ed4-124">None</span></span> | <span data-ttu-id="14ed4-125">指定した検索フォルダーを削除します。</span><span class="sxs-lookup"><span data-stu-id="14ed4-125">Delete the specified search folder.</span></span> |
| [<span data-ttu-id="14ed4-126">検索フォルダー内のすべてのメッセージを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="14ed4-126">List all messages in a search folder</span></span>](../api/mailfolder-list-messages.md) | <span data-ttu-id="14ed4-127">[message](message.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="14ed4-127">[message](message.md) collection</span></span> | <span data-ttu-id="14ed4-128">指定した検索フォルダー内のすべてのメッセージを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="14ed4-128">List all the messages in the specified search folder.</span></span> |

## <a name="properties"></a><span data-ttu-id="14ed4-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14ed4-129">Properties</span></span>

| <span data-ttu-id="14ed4-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14ed4-130">Property</span></span> | <span data-ttu-id="14ed4-131">型</span><span class="sxs-lookup"><span data-stu-id="14ed4-131">Type</span></span> | <span data-ttu-id="14ed4-132">説明</span><span class="sxs-lookup"><span data-stu-id="14ed4-132">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="14ed4-133">参照して</span><span class="sxs-lookup"><span data-stu-id="14ed4-133">isSupported</span></span> | <span data-ttu-id="14ed4-134">ブール値</span><span class="sxs-lookup"><span data-stu-id="14ed4-134">Boolean</span></span> | <span data-ttu-id="14ed4-135">検索フォルダーは、REST Api を使用して編集可能かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="14ed4-135">Indicates whether a search folder is editable using REST APIs.</span></span> |
| <span data-ttu-id="14ed4-136">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="14ed4-136">includeNestedFolders</span></span> | <span data-ttu-id="14ed4-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="14ed4-137">Boolean</span></span> | <span data-ttu-id="14ed4-138">メールボックス フォルダー階層を走査する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="14ed4-138">Indicates how the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="14ed4-139">`true`詳細検索をする必要があることを意味時に`false`簡易検索を代わりに行う必要があることを意味します。</span><span class="sxs-lookup"><span data-stu-id="14ed4-139">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="14ed4-140">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="14ed4-140">sourceFolderIDs</span></span> | <span data-ttu-id="14ed4-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="14ed4-141">String collection</span></span> | <span data-ttu-id="14ed4-142">メールボックス フォルダーをマイニングする必要があります。</span><span class="sxs-lookup"><span data-stu-id="14ed4-142">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="14ed4-143">filterQuery</span><span class="sxs-lookup"><span data-stu-id="14ed4-143">filterQuery</span></span> | <span data-ttu-id="14ed4-144">String</span><span class="sxs-lookup"><span data-stu-id="14ed4-144">String</span></span> | <span data-ttu-id="14ed4-145">メッセージをフィルタ リングする OData クエリです。</span><span class="sxs-lookup"><span data-stu-id="14ed4-145">The OData query to filter the messages.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="14ed4-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="14ed4-146">JSON representation</span></span>

<span data-ttu-id="14ed4-147">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="14ed4-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailSearchFolder"
}-->

```json
{
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": ["string"],
  "filterQuery": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2018-01-23 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailSearchFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mailsearchfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
