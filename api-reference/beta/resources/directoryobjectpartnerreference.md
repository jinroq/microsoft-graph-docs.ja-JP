---
title: directoryObjectPartnerReference リソースの種類
description: パートナーテナント内のディレクトリオブジェクトへの参照を表します。 directoryObject から継承します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 327528f41795360e0da109b513f3f3f08ac0b268
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657932"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="7a678-104">directoryObjectPartnerReference リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7a678-104">directoryObjectPartnerReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a678-105">パートナー組織内のディレクトリオブジェクトへの参照を表します。</span><span class="sxs-lookup"><span data-stu-id="7a678-105">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="7a678-106">[directoryObject](directoryobject.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="7a678-106">Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7a678-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a678-107">Properties</span></span>

| <span data-ttu-id="7a678-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a678-108">Property</span></span> | <span data-ttu-id="7a678-109">型</span><span class="sxs-lookup"><span data-stu-id="7a678-109">Type</span></span> | <span data-ttu-id="7a678-110">説明</span><span class="sxs-lookup"><span data-stu-id="7a678-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7a678-111">description</span><span class="sxs-lookup"><span data-stu-id="7a678-111">description</span></span>|<span data-ttu-id="7a678-112">String</span><span class="sxs-lookup"><span data-stu-id="7a678-112">String</span></span>| <span data-ttu-id="7a678-113">返されるオブジェクトの説明。</span><span class="sxs-lookup"><span data-stu-id="7a678-113">Description of the object returned.</span></span> <span data-ttu-id="7a678-114">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7a678-114">Read-only.</span></span> |
|<span data-ttu-id="7a678-115">displayName</span><span class="sxs-lookup"><span data-stu-id="7a678-115">displayName</span></span>|<span data-ttu-id="7a678-116">String</span><span class="sxs-lookup"><span data-stu-id="7a678-116">String</span></span>| <span data-ttu-id="7a678-117">グループまたはアプリケーションなど、返されるディレクトリオブジェクトの名前。</span><span class="sxs-lookup"><span data-stu-id="7a678-117">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="7a678-118">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7a678-118">Read-only.</span></span> |
|<span data-ttu-id="7a678-119">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="7a678-119">externalPartnerTenantId</span></span>|<span data-ttu-id="7a678-120">Guid</span><span class="sxs-lookup"><span data-stu-id="7a678-120">Guid</span></span>| <span data-ttu-id="7a678-121">パートナーテナントのテナント識別子。</span><span class="sxs-lookup"><span data-stu-id="7a678-121">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="7a678-122">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7a678-122">Read-only.</span></span> |
|<span data-ttu-id="7a678-123">id</span><span class="sxs-lookup"><span data-stu-id="7a678-123">id</span></span>|<span data-ttu-id="7a678-124">文字列</span><span class="sxs-lookup"><span data-stu-id="7a678-124">String</span></span>| <span data-ttu-id="7a678-125">リソースの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="7a678-125">The unique identifier for the resource.</span></span> <span data-ttu-id="7a678-126">[directoryObject](directoryobject.md) から継承されます。</span><span class="sxs-lookup"><span data-stu-id="7a678-126">Inherited from [directoryObject](directoryobject.md).</span></span> <span data-ttu-id="7a678-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7a678-127">Read-only.</span></span> |
|<span data-ttu-id="7a678-128">objectType</span><span class="sxs-lookup"><span data-stu-id="7a678-128">objectType</span></span>|<span data-ttu-id="7a678-129">文字列</span><span class="sxs-lookup"><span data-stu-id="7a678-129">String</span></span>| <span data-ttu-id="7a678-130">パートナーテナント内の参照されるオブジェクトの種類。</span><span class="sxs-lookup"><span data-stu-id="7a678-130">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="7a678-131">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7a678-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7a678-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7a678-132">JSON representation</span></span>

<span data-ttu-id="7a678-133">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7a678-133">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="7a678-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="7a678-134">See also</span></span>

- [<span data-ttu-id="7a678-135">ID のリストからディレクトリ オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="7a678-135">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

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
