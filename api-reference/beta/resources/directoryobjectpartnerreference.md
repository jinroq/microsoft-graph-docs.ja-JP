---
title: directoryObjectPartnerReference リソースの種類
description: パートナー テナント内のディレクトリ オブジェクトへの参照を表します。 directoryObject から継承します。
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 46d0f749ac77e7d51e03314e78cfccf494dcc6fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884862"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="26623-104">directoryObjectPartnerReference リソースの種類</span><span class="sxs-lookup"><span data-stu-id="26623-104">directoryObjectPartnerReference resource type</span></span>

> <span data-ttu-id="26623-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="26623-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26623-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26623-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="26623-107">パートナー組織内のディレクトリ オブジェクトへの参照を表します。</span><span class="sxs-lookup"><span data-stu-id="26623-107">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="26623-108">[directoryObject](directoryobject.md?view=graph-rest-beta) から継承します。</span><span class="sxs-lookup"><span data-stu-id="26623-108">Inherits from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span>

## <a name="properties"></a><span data-ttu-id="26623-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26623-109">Properties</span></span>

| <span data-ttu-id="26623-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26623-110">Property</span></span> | <span data-ttu-id="26623-111">種類</span><span class="sxs-lookup"><span data-stu-id="26623-111">Type</span></span> | <span data-ttu-id="26623-112">説明</span><span class="sxs-lookup"><span data-stu-id="26623-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="26623-113">説明</span><span class="sxs-lookup"><span data-stu-id="26623-113">description</span></span>|<span data-ttu-id="26623-114">String</span><span class="sxs-lookup"><span data-stu-id="26623-114">String</span></span>| <span data-ttu-id="26623-115">オブジェクトの説明が返されます。</span><span class="sxs-lookup"><span data-stu-id="26623-115">Description of the object returned.</span></span> <span data-ttu-id="26623-116">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="26623-116">Read-only.</span></span> |
|<span data-ttu-id="26623-117">displayName</span><span class="sxs-lookup"><span data-stu-id="26623-117">displayName</span></span>|<span data-ttu-id="26623-118">String</span><span class="sxs-lookup"><span data-stu-id="26623-118">String</span></span>| <span data-ttu-id="26623-119">グループまたはアプリケーションのように、返されるディレクトリ オブジェクトの名前です。</span><span class="sxs-lookup"><span data-stu-id="26623-119">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="26623-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="26623-120">Read-only.</span></span> |
|<span data-ttu-id="26623-121">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="26623-121">externalPartnerTenantId</span></span>|<span data-ttu-id="26623-122">Guid</span><span class="sxs-lookup"><span data-stu-id="26623-122">Guid</span></span>| <span data-ttu-id="26623-123">パートナー テナントにテナントの識別子です。</span><span class="sxs-lookup"><span data-stu-id="26623-123">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="26623-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="26623-124">Read-only.</span></span> |
|<span data-ttu-id="26623-125">id</span><span class="sxs-lookup"><span data-stu-id="26623-125">id</span></span>|<span data-ttu-id="26623-126">String</span><span class="sxs-lookup"><span data-stu-id="26623-126">String</span></span>| <span data-ttu-id="26623-127">リソースの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="26623-127">The unique identifier for the resource.</span></span> <span data-ttu-id="26623-128">[directoryObject](directoryobject.md?view=graph-rest-beta) から継承されます。</span><span class="sxs-lookup"><span data-stu-id="26623-128">Inherited from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span> <span data-ttu-id="26623-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="26623-129">Read-only.</span></span> |
|<span data-ttu-id="26623-130">objectType</span><span class="sxs-lookup"><span data-stu-id="26623-130">objectType</span></span>|<span data-ttu-id="26623-131">String</span><span class="sxs-lookup"><span data-stu-id="26623-131">String</span></span>| <span data-ttu-id="26623-132">パートナー テナントで参照されるオブジェクトの型。</span><span class="sxs-lookup"><span data-stu-id="26623-132">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="26623-133">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="26623-133">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="26623-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="26623-134">JSON representation</span></span>

<span data-ttu-id="26623-135">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="26623-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObjectPartnerReference"
}-->

```json
{
  "description": "string ",
  "displayName": "string",
  "externalPartnerTenantId": "string (identifier)",
  "id": "string (identifier)",
  "objectType": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="26623-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="26623-136">See also</span></span>

- [<span data-ttu-id="26623-137">ID のリストからディレクトリ オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="26623-137">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

<!-- uuid: fbec8cd7-cfe4-431d-87fc-d102cd2841a4
2018-12-06 02:01:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
