---
title: 履歴リソースの種類
description: Dynamics 365 Business Central のジャーナル。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 7cfc723a4370c2b30440dcd4e33b50ed066ac89b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006593"
---
# <a name="journal-resource-type"></a><span data-ttu-id="b0fc0-103">履歴リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b0fc0-103">journal resource type</span></span>
<span data-ttu-id="b0fc0-104">Dynamics 365 Business Central のジャーナルを表します。</span><span class="sxs-lookup"><span data-stu-id="b0fc0-104">Represents a journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="b0fc0-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="b0fc0-105">Methods</span></span>

| <span data-ttu-id="b0fc0-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="b0fc0-106">Method</span></span>                                            |<span data-ttu-id="b0fc0-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b0fc0-107">Return Type</span></span>|<span data-ttu-id="b0fc0-108">説明</span><span class="sxs-lookup"><span data-stu-id="b0fc0-108">Description</span></span>    |
|:--------------------------------------------------|:----------|:--------------|
|[<span data-ttu-id="b0fc0-109">仕訳帳を取得する</span><span class="sxs-lookup"><span data-stu-id="b0fc0-109">Get journal</span></span>](../api/dynamics-journal-get.md)      |<span data-ttu-id="b0fc0-110">雑誌</span><span class="sxs-lookup"><span data-stu-id="b0fc0-110">journal</span></span>    |<span data-ttu-id="b0fc0-111">ジャーナルを取得します。</span><span class="sxs-lookup"><span data-stu-id="b0fc0-111">Gets a journal.</span></span>   |
|[<span data-ttu-id="b0fc0-112">仕訳帳の投稿</span><span class="sxs-lookup"><span data-stu-id="b0fc0-112">Post journal</span></span>](../api/dynamics-create-journal.md)  |<span data-ttu-id="b0fc0-113">雑誌</span><span class="sxs-lookup"><span data-stu-id="b0fc0-113">journal</span></span>    |<span data-ttu-id="b0fc0-114">仕訳帳を作成します。</span><span class="sxs-lookup"><span data-stu-id="b0fc0-114">Creates a journal.</span></span>|
|[<span data-ttu-id="b0fc0-115">Patch ジャーナル</span><span class="sxs-lookup"><span data-stu-id="b0fc0-115">Patch journal</span></span>](../api/dynamics-journal-update.md) |<span data-ttu-id="b0fc0-116">雑誌</span><span class="sxs-lookup"><span data-stu-id="b0fc0-116">journal</span></span>    |<span data-ttu-id="b0fc0-117">仕訳帳を更新します。</span><span class="sxs-lookup"><span data-stu-id="b0fc0-117">Updates a journal.</span></span>|
|[<span data-ttu-id="b0fc0-118">仕訳帳を削除する</span><span class="sxs-lookup"><span data-stu-id="b0fc0-118">Delete journal</span></span>](../api/dynamics-journal-delete.md)|<span data-ttu-id="b0fc0-119">none</span><span class="sxs-lookup"><span data-stu-id="b0fc0-119">none</span></span>       |<span data-ttu-id="b0fc0-120">仕訳帳を削除します。</span><span class="sxs-lookup"><span data-stu-id="b0fc0-120">Deletes a journal.</span></span>|

## <a name="properties"></a><span data-ttu-id="b0fc0-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0fc0-121">Properties</span></span>
| <span data-ttu-id="b0fc0-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0fc0-122">Property</span></span>           | <span data-ttu-id="b0fc0-123">型</span><span class="sxs-lookup"><span data-stu-id="b0fc0-123">Type</span></span>                  |<span data-ttu-id="b0fc0-124">説明</span><span class="sxs-lookup"><span data-stu-id="b0fc0-124">Description</span></span>                                           |
|:-------------------|:----------------------|:-----------------------------------------------------|
|<span data-ttu-id="b0fc0-125">id</span><span class="sxs-lookup"><span data-stu-id="b0fc0-125">id</span></span>                  |<span data-ttu-id="b0fc0-126">GUID</span><span class="sxs-lookup"><span data-stu-id="b0fc0-126">GUID</span></span>                   |<span data-ttu-id="b0fc0-127">ジャーナルの一意の ID。</span><span class="sxs-lookup"><span data-stu-id="b0fc0-127">The unique ID of the journal.</span></span> <span data-ttu-id="b0fc0-128">編集できません。</span><span class="sxs-lookup"><span data-stu-id="b0fc0-128">Non-editable.</span></span>           |
|<span data-ttu-id="b0fc0-129">code</span><span class="sxs-lookup"><span data-stu-id="b0fc0-129">code</span></span>                |<span data-ttu-id="b0fc0-130">文字列、最大サイズ10</span><span class="sxs-lookup"><span data-stu-id="b0fc0-130">string, maximum size 10</span></span>| <span data-ttu-id="b0fc0-131">ジャーナルのコード。</span><span class="sxs-lookup"><span data-stu-id="b0fc0-131">The code of the journal.</span></span>                             |
|<span data-ttu-id="b0fc0-132">displayName</span><span class="sxs-lookup"><span data-stu-id="b0fc0-132">displayName</span></span>         |<span data-ttu-id="b0fc0-133">文字列、最大サイズ50</span><span class="sxs-lookup"><span data-stu-id="b0fc0-133">string, maximum size 50</span></span>| <span data-ttu-id="b0fc0-134">仕訳帳の表示名。</span><span class="sxs-lookup"><span data-stu-id="b0fc0-134">The display name of the journal.</span></span>                     |
|<span data-ttu-id="b0fc0-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0fc0-135">lastModifiedDateTime</span></span>|<span data-ttu-id="b0fc0-136">datetime</span><span class="sxs-lookup"><span data-stu-id="b0fc0-136">datetime</span></span>               |<span data-ttu-id="b0fc0-137">ジャーナルが変更された最後の datetime。</span><span class="sxs-lookup"><span data-stu-id="b0fc0-137">The last datetime the journal was modified.</span></span> <span data-ttu-id="b0fc0-138">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b0fc0-138">Read-Only.</span></span>|

## <a name="bound-actions"></a><span data-ttu-id="b0fc0-139">バインドされたアクション</span><span class="sxs-lookup"><span data-stu-id="b0fc0-139">Bound actions</span></span>
<span data-ttu-id="b0fc0-140">ジャーナルリソースの種類は、と呼ば`post`れる、対応する一般的なジャーナルバッチを投稿するバインドアクションを提供します。</span><span class="sxs-lookup"><span data-stu-id="b0fc0-140">The journal resource type offers a bound action called `post` which posts the corresponding general journal batch.</span></span>

<span data-ttu-id="b0fc0-141">次の例に、一般的なジャーナルバッチの投稿を示します。</span><span class="sxs-lookup"><span data-stu-id="b0fc0-141">Posting the general journal batch is illustrated in the following example:</span></span>  
<span data-ttu-id="b0fc0-142">`POST https://graph.microsoft.com/beta/financials/companies{id}/journals{id}/post`.</span><span class="sxs-lookup"><span data-stu-id="b0fc0-142"></span></span>

<span data-ttu-id="b0fc0-143">応答にはコンテンツがありません。応答コードは204です。</span><span class="sxs-lookup"><span data-stu-id="b0fc0-143">The response has no content; the response code is 204.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0fc0-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b0fc0-144">JSON representation</span></span>

<span data-ttu-id="b0fc0-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b0fc0-145">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```

