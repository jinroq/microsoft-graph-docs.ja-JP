---
title: directoryobjectpartnerreference リソースの種類
description: パートナーテナント内のディレクトリオブジェクトへの参照を表します。 directoryObject から継承します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 658571ce406e74b78a6924ed0290ab672c791e94
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341737"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="e82ce-104">directoryobjectpartnerreference リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e82ce-104">directoryObjectPartnerReference resource type</span></span>

<span data-ttu-id="e82ce-105">パートナー組織内のディレクトリオブジェクトへの参照を表します。</span><span class="sxs-lookup"><span data-stu-id="e82ce-105">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="e82ce-106">[directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) から継承します。</span><span class="sxs-lookup"><span data-stu-id="e82ce-106">Inherits from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span></span>

## <a name="properties"></a><span data-ttu-id="e82ce-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e82ce-107">Properties</span></span>

| <span data-ttu-id="e82ce-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e82ce-108">Property</span></span> | <span data-ttu-id="e82ce-109">型</span><span class="sxs-lookup"><span data-stu-id="e82ce-109">Type</span></span> | <span data-ttu-id="e82ce-110">説明</span><span class="sxs-lookup"><span data-stu-id="e82ce-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e82ce-111">description</span><span class="sxs-lookup"><span data-stu-id="e82ce-111">description</span></span>|<span data-ttu-id="e82ce-112">String</span><span class="sxs-lookup"><span data-stu-id="e82ce-112">String</span></span>| <span data-ttu-id="e82ce-113">返されるオブジェクトの説明。</span><span class="sxs-lookup"><span data-stu-id="e82ce-113">Description of the object returned.</span></span> <span data-ttu-id="e82ce-114">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e82ce-114">Read-only.</span></span> |
|<span data-ttu-id="e82ce-115">displayName</span><span class="sxs-lookup"><span data-stu-id="e82ce-115">displayName</span></span>|<span data-ttu-id="e82ce-116">String</span><span class="sxs-lookup"><span data-stu-id="e82ce-116">String</span></span>| <span data-ttu-id="e82ce-117">グループまたはアプリケーションなど、返されるディレクトリオブジェクトの名前。</span><span class="sxs-lookup"><span data-stu-id="e82ce-117">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="e82ce-118">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e82ce-118">Read-only.</span></span> |
|<span data-ttu-id="e82ce-119">externalpartnertenantid</span><span class="sxs-lookup"><span data-stu-id="e82ce-119">externalPartnerTenantId</span></span>|<span data-ttu-id="e82ce-120">Guid</span><span class="sxs-lookup"><span data-stu-id="e82ce-120">Guid</span></span>| <span data-ttu-id="e82ce-121">パートナーテナントのテナント識別子。</span><span class="sxs-lookup"><span data-stu-id="e82ce-121">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="e82ce-122">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="e82ce-122">Read-only.</span></span> |
|<span data-ttu-id="e82ce-123">id</span><span class="sxs-lookup"><span data-stu-id="e82ce-123">id</span></span>|<span data-ttu-id="e82ce-124">String</span><span class="sxs-lookup"><span data-stu-id="e82ce-124">String</span></span>| <span data-ttu-id="e82ce-125">リソースの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="e82ce-125">The unique identifier for the resource.</span></span> <span data-ttu-id="e82ce-126">[directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e82ce-126">Inherited from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span></span> <span data-ttu-id="e82ce-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e82ce-127">Read-only.</span></span> |
|<span data-ttu-id="e82ce-128">objectType</span><span class="sxs-lookup"><span data-stu-id="e82ce-128">objectType</span></span>|<span data-ttu-id="e82ce-129">文字列</span><span class="sxs-lookup"><span data-stu-id="e82ce-129">String</span></span>| <span data-ttu-id="e82ce-130">パートナーテナント内の参照されるオブジェクトの種類。</span><span class="sxs-lookup"><span data-stu-id="e82ce-130">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="e82ce-131">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e82ce-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e82ce-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e82ce-132">JSON representation</span></span>

<span data-ttu-id="e82ce-133">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e82ce-133">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="e82ce-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="e82ce-134">See also</span></span>

- [<span data-ttu-id="e82ce-135">ID のリストからディレクトリ オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="e82ce-135">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-v1.0)

<!-- uuid: fbec8cd7-cfe4-431d-87fc-d102cd2841a4
2018-12-06 02:01:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
