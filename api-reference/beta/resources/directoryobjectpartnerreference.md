---
title: directoryObjectPartnerReference リソースの種類
description: パートナーテナント内のディレクトリオブジェクトへの参照を表します。 directoryObject から継承します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 54a6d742e31dba6861bed55d26179e1936fa8c5d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973834"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="62268-104">directoryObjectPartnerReference リソースの種類</span><span class="sxs-lookup"><span data-stu-id="62268-104">directoryObjectPartnerReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62268-105">パートナー組織内のディレクトリオブジェクトへの参照を表します。</span><span class="sxs-lookup"><span data-stu-id="62268-105">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="62268-106">[directoryObject](directoryobject.md) から継承します。</span><span class="sxs-lookup"><span data-stu-id="62268-106">Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="properties"></a><span data-ttu-id="62268-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62268-107">Properties</span></span>

| <span data-ttu-id="62268-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62268-108">Property</span></span> | <span data-ttu-id="62268-109">型</span><span class="sxs-lookup"><span data-stu-id="62268-109">Type</span></span> | <span data-ttu-id="62268-110">説明</span><span class="sxs-lookup"><span data-stu-id="62268-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="62268-111">description</span><span class="sxs-lookup"><span data-stu-id="62268-111">description</span></span>|<span data-ttu-id="62268-112">String</span><span class="sxs-lookup"><span data-stu-id="62268-112">String</span></span>| <span data-ttu-id="62268-113">返されるオブジェクトの説明。</span><span class="sxs-lookup"><span data-stu-id="62268-113">Description of the object returned.</span></span> <span data-ttu-id="62268-114">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="62268-114">Read-only.</span></span> |
|<span data-ttu-id="62268-115">displayName</span><span class="sxs-lookup"><span data-stu-id="62268-115">displayName</span></span>|<span data-ttu-id="62268-116">String</span><span class="sxs-lookup"><span data-stu-id="62268-116">String</span></span>| <span data-ttu-id="62268-117">グループまたはアプリケーションなど、返されるディレクトリオブジェクトの名前。</span><span class="sxs-lookup"><span data-stu-id="62268-117">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="62268-118">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="62268-118">Read-only.</span></span> |
|<span data-ttu-id="62268-119">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="62268-119">externalPartnerTenantId</span></span>|<span data-ttu-id="62268-120">Guid</span><span class="sxs-lookup"><span data-stu-id="62268-120">Guid</span></span>| <span data-ttu-id="62268-121">パートナーテナントのテナント識別子。</span><span class="sxs-lookup"><span data-stu-id="62268-121">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="62268-122">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="62268-122">Read-only.</span></span> |
|<span data-ttu-id="62268-123">id</span><span class="sxs-lookup"><span data-stu-id="62268-123">id</span></span>|<span data-ttu-id="62268-124">文字列</span><span class="sxs-lookup"><span data-stu-id="62268-124">String</span></span>| <span data-ttu-id="62268-125">リソースの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="62268-125">The unique identifier for the resource.</span></span> <span data-ttu-id="62268-126">[directoryObject](directoryobject.md) から継承されます。</span><span class="sxs-lookup"><span data-stu-id="62268-126">Inherited from [directoryObject](directoryobject.md).</span></span> <span data-ttu-id="62268-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="62268-127">Read-only.</span></span> |
|<span data-ttu-id="62268-128">objectType</span><span class="sxs-lookup"><span data-stu-id="62268-128">objectType</span></span>|<span data-ttu-id="62268-129">文字列</span><span class="sxs-lookup"><span data-stu-id="62268-129">String</span></span>| <span data-ttu-id="62268-130">パートナーテナント内の参照されるオブジェクトの種類。</span><span class="sxs-lookup"><span data-stu-id="62268-130">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="62268-131">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="62268-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="62268-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="62268-132">JSON representation</span></span>

<span data-ttu-id="62268-133">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="62268-133">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="62268-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="62268-134">See also</span></span>

- [<span data-ttu-id="62268-135">ID のリストからディレクトリ オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="62268-135">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

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
