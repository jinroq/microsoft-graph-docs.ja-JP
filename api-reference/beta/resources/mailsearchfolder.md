---
title: mailSearchFolder リソースの種類
description: MailSearchFolder は、指定した検索条件に一致するすべての電子メールアイテムを含む、ユーザーのメールボックス内の仮想フォルダーです。 mailSearchFolder は mailFolder から継承します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f709347d8ba81a5b42ab512a80beae8780805f2f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009847"
---
# <a name="mailsearchfolder-resource-type"></a><span data-ttu-id="3bf62-104">mailSearchFolder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3bf62-104">mailSearchFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bf62-105">**Mailsearchfolder**は、指定した検索条件に一致するすべての電子メールアイテムを含む、ユーザーのメールボックス内の仮想フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="3bf62-105">A **mailSearchFolder** is a virtual folder in the user's mailbox that contains all the email items matching specified search criteria.</span></span> <span data-ttu-id="3bf62-106">**Mailsearchfolder**は[mailfolder](mailfolder.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="3bf62-106">**mailSearchFolder** inherits from [mailFolder](mailfolder.md).</span></span> <span data-ttu-id="3bf62-107">検索フォルダーは、ユーザーの Exchange Online メールボックス内の任意のフォルダーに作成できます。</span><span class="sxs-lookup"><span data-stu-id="3bf62-107">Search folders can be created in any folder in a user's Exchange Online mailbox.</span></span> <span data-ttu-id="3bf62-108">ただし、検索フォルダーが Outlook、web 用の Outlook、または Outlook Live に表示されるようにするには、 **WellKnownFolderName**フォルダー内にフォルダーを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3bf62-108">However, for a search folder to appear in Outlook, Outlook for the web, or Outlook Live, the folder must be created in the **WellKnownFolderName.SearchFolders** folder.</span></span> 

## <a name="search-folder-lifecycle"></a><span data-ttu-id="3bf62-109">検索フォルダーのライフサイクル</span><span class="sxs-lookup"><span data-stu-id="3bf62-109">Search folder lifecycle</span></span>

<span data-ttu-id="3bf62-110">アプリケーションによって作成された検索フォルダーは、次のいずれかの理由により、Exchange Online で削除できます。</span><span class="sxs-lookup"><span data-stu-id="3bf62-110">Search folders created by your application can be deleted by Exchange Online for one of the following reasons:</span></span>

1.  <span data-ttu-id="3bf62-111">検索フォルダーは利用できなくなってから45日後に有効期限が切れます。</span><span class="sxs-lookup"><span data-stu-id="3bf62-111">Search folders expire after 45 days of no usage.</span></span> 
2.  <span data-ttu-id="3bf62-112">ソースフォルダーごとに作成できる検索フォルダーの数には制限があります。</span><span class="sxs-lookup"><span data-stu-id="3bf62-112">There are limits on the number of search folders that can be created per source folder.</span></span> <span data-ttu-id="3bf62-113">この制限が侵害された場合は、古い検索フォルダーが削除され、新しいフォルダーを使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="3bf62-113">When this limit is breached, older search folders are deleted to make way for new ones.</span></span> 

<span data-ttu-id="3bf62-114">検索フォルダーが削除されると、アプリは新しい検索フォルダーリソースを作成して同じものを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3bf62-114">When a search folder is deleted, your app should create a new search folder resource and use the same.</span></span>


## <a name="methods"></a><span data-ttu-id="3bf62-115">メソッド</span><span class="sxs-lookup"><span data-stu-id="3bf62-115">Methods</span></span>

| <span data-ttu-id="3bf62-116">メソッド</span><span class="sxs-lookup"><span data-stu-id="3bf62-116">Method</span></span> | <span data-ttu-id="3bf62-117">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3bf62-117">Return Type</span></span>  | <span data-ttu-id="3bf62-118">説明</span><span class="sxs-lookup"><span data-stu-id="3bf62-118">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="3bf62-119">検索フォルダーを作成する</span><span class="sxs-lookup"><span data-stu-id="3bf62-119">Create a search folder</span></span>](../api/mailsearchfolder-post.md) | [<span data-ttu-id="3bf62-120">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="3bf62-120">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="3bf62-121">このユーザーのメールボックスに検索フォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="3bf62-121">Create a search folder in this user's mailbox.</span></span> |
| [<span data-ttu-id="3bf62-122">検索フォルダーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="3bf62-122">List search folders</span></span>](../api/mailfolder-list-childfolders.md) | <span data-ttu-id="3bf62-123">[mailFolder](mailfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3bf62-123">[mailFolder](mailfolder.md) collection</span></span> | <span data-ttu-id="3bf62-124">このユーザーのメールボックス内のすべてのフォルダー (検索フォルダーを含む) を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="3bf62-124">List all the folders in this user's mailbox, including search folders.</span></span> |
| [<span data-ttu-id="3bf62-125">検索フォルダ―を取得する</span><span class="sxs-lookup"><span data-stu-id="3bf62-125">Get a search folder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="3bf62-126">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="3bf62-126">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="3bf62-127">指定した検索フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="3bf62-127">Get the specified search folder.</span></span> |
| [<span data-ttu-id="3bf62-128">検索フォルダーを更新する</span><span class="sxs-lookup"><span data-stu-id="3bf62-128">Update a search folder</span></span>](../api/mailsearchfolder-update.md) | [<span data-ttu-id="3bf62-129">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="3bf62-129">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="3bf62-130">指定した検索フォルダーを更新します。</span><span class="sxs-lookup"><span data-stu-id="3bf62-130">Update the specified search folder.</span></span> |
| [<span data-ttu-id="3bf62-131">検索フォルダーを削除する</span><span class="sxs-lookup"><span data-stu-id="3bf62-131">Delete a search folder</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="3bf62-132">None</span><span class="sxs-lookup"><span data-stu-id="3bf62-132">None</span></span> | <span data-ttu-id="3bf62-133">指定した検索フォルダーを削除します。</span><span class="sxs-lookup"><span data-stu-id="3bf62-133">Delete the specified search folder.</span></span> |
| [<span data-ttu-id="3bf62-134">検索フォルダー内のすべてのメッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="3bf62-134">List all messages in a search folder</span></span>](../api/mailfolder-list-messages.md) | <span data-ttu-id="3bf62-135">[message](message.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3bf62-135">[message](message.md) collection</span></span> | <span data-ttu-id="3bf62-136">指定した検索フォルダー内のすべてのメッセージを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="3bf62-136">List all the messages in the specified search folder.</span></span> |

## <a name="properties"></a><span data-ttu-id="3bf62-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3bf62-137">Properties</span></span>

| <span data-ttu-id="3bf62-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3bf62-138">Property</span></span> | <span data-ttu-id="3bf62-139">型</span><span class="sxs-lookup"><span data-stu-id="3bf62-139">Type</span></span> | <span data-ttu-id="3bf62-140">説明</span><span class="sxs-lookup"><span data-stu-id="3bf62-140">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="3bf62-141">isSupported</span><span class="sxs-lookup"><span data-stu-id="3bf62-141">isSupported</span></span> | <span data-ttu-id="3bf62-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bf62-142">Boolean</span></span> | <span data-ttu-id="3bf62-143">検索フォルダーが REST Api を使用して編集可能かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3bf62-143">Indicates whether a search folder is editable using REST APIs.</span></span> |
| <span data-ttu-id="3bf62-144">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="3bf62-144">includeNestedFolders</span></span> | <span data-ttu-id="3bf62-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bf62-145">Boolean</span></span> | <span data-ttu-id="3bf62-146">検索でメールボックスフォルダー階層をスキャンする方法を示します。</span><span class="sxs-lookup"><span data-stu-id="3bf62-146">Indicates how the mailbox folder hierarchy should be traversed in the search.</span></span> <span data-ttu-id="3bf62-147">`true`**sourceFolderIds**で明示的に指定された各フォルダーの階層内に子フォルダーを含めるには、詳細検索を実行する必要があることを意味します。</span><span class="sxs-lookup"><span data-stu-id="3bf62-147">`true` means that a deep search should be done to include child folders in the hierarchy of each folder explicitly specified in **sourceFolderIds**.</span></span> <span data-ttu-id="3bf62-148">`false`は、 **sourceFolderIds**で明示的に指定された各フォルダーの浅い検索を意味します。</span><span class="sxs-lookup"><span data-stu-id="3bf62-148">`false` means a shallow search of only each of the folders explicitly specified in **sourceFolderIds**.</span></span> |
| <span data-ttu-id="3bf62-149">sourceFolderIds</span><span class="sxs-lookup"><span data-stu-id="3bf62-149">sourceFolderIds</span></span> | <span data-ttu-id="3bf62-150">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="3bf62-150">String collection</span></span> | <span data-ttu-id="3bf62-151">マイニングするメールボックスフォルダー。</span><span class="sxs-lookup"><span data-stu-id="3bf62-151">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="3bf62-152">filterQuery</span><span class="sxs-lookup"><span data-stu-id="3bf62-152">filterQuery</span></span> | <span data-ttu-id="3bf62-153">String</span><span class="sxs-lookup"><span data-stu-id="3bf62-153">String</span></span> | <span data-ttu-id="3bf62-154">メッセージをフィルター処理するための OData クエリ。</span><span class="sxs-lookup"><span data-stu-id="3bf62-154">The OData query to filter the messages.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3bf62-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3bf62-155">JSON representation</span></span>

<span data-ttu-id="3bf62-156">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3bf62-156">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailSearchFolder"
}-->

```json
{
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIds": ["string"],
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
  "suppressions": []
}
-->
