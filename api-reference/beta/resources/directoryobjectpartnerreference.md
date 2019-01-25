---
title: directoryObjectPartnerReference リソースの種類
description: パートナー テナント内のディレクトリ オブジェクトへの参照を表します。 directoryObject から継承します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a031586d1f92bf2b8b331e9b71058211b4617382
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511052"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="c77e1-104">directoryObjectPartnerReference リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c77e1-104">directoryObjectPartnerReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c77e1-105">パートナー組織内のディレクトリ オブジェクトへの参照を表します。</span><span class="sxs-lookup"><span data-stu-id="c77e1-105">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="c77e1-106">[directoryObject](directoryobject.md?view=graph-rest-beta) から継承します。</span><span class="sxs-lookup"><span data-stu-id="c77e1-106">Inherits from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span>

## <a name="properties"></a><span data-ttu-id="c77e1-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c77e1-107">Properties</span></span>

| <span data-ttu-id="c77e1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c77e1-108">Property</span></span> | <span data-ttu-id="c77e1-109">型</span><span class="sxs-lookup"><span data-stu-id="c77e1-109">Type</span></span> | <span data-ttu-id="c77e1-110">説明</span><span class="sxs-lookup"><span data-stu-id="c77e1-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c77e1-111">説明</span><span class="sxs-lookup"><span data-stu-id="c77e1-111">description</span></span>|<span data-ttu-id="c77e1-112">文字列</span><span class="sxs-lookup"><span data-stu-id="c77e1-112">String</span></span>| <span data-ttu-id="c77e1-113">オブジェクトの説明が返されます。</span><span class="sxs-lookup"><span data-stu-id="c77e1-113">Description of the object returned.</span></span> <span data-ttu-id="c77e1-114">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c77e1-114">Read-only.</span></span> |
|<span data-ttu-id="c77e1-115">displayName</span><span class="sxs-lookup"><span data-stu-id="c77e1-115">displayName</span></span>|<span data-ttu-id="c77e1-116">String</span><span class="sxs-lookup"><span data-stu-id="c77e1-116">String</span></span>| <span data-ttu-id="c77e1-117">グループまたはアプリケーションのように、返されるディレクトリ オブジェクトの名前です。</span><span class="sxs-lookup"><span data-stu-id="c77e1-117">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="c77e1-118">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c77e1-118">Read-only.</span></span> |
|<span data-ttu-id="c77e1-119">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="c77e1-119">externalPartnerTenantId</span></span>|<span data-ttu-id="c77e1-120">Guid</span><span class="sxs-lookup"><span data-stu-id="c77e1-120">Guid</span></span>| <span data-ttu-id="c77e1-121">パートナー テナントにテナントの識別子です。</span><span class="sxs-lookup"><span data-stu-id="c77e1-121">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="c77e1-122">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="c77e1-122">Read-only.</span></span> |
|<span data-ttu-id="c77e1-123">id</span><span class="sxs-lookup"><span data-stu-id="c77e1-123">id</span></span>|<span data-ttu-id="c77e1-124">文字列</span><span class="sxs-lookup"><span data-stu-id="c77e1-124">String</span></span>| <span data-ttu-id="c77e1-125">リソースの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="c77e1-125">The unique identifier for the resource.</span></span> <span data-ttu-id="c77e1-126">[directoryObject](directoryobject.md?view=graph-rest-beta) から継承されます。</span><span class="sxs-lookup"><span data-stu-id="c77e1-126">Inherited from [directoryObject](directoryobject.md?view=graph-rest-beta).</span></span> <span data-ttu-id="c77e1-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c77e1-127">Read-only.</span></span> |
|<span data-ttu-id="c77e1-128">objectType</span><span class="sxs-lookup"><span data-stu-id="c77e1-128">objectType</span></span>|<span data-ttu-id="c77e1-129">String</span><span class="sxs-lookup"><span data-stu-id="c77e1-129">String</span></span>| <span data-ttu-id="c77e1-130">パートナー テナントで参照されるオブジェクトの型。</span><span class="sxs-lookup"><span data-stu-id="c77e1-130">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="c77e1-131">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c77e1-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c77e1-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c77e1-132">JSON representation</span></span>

<span data-ttu-id="c77e1-133">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c77e1-133">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="c77e1-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="c77e1-134">See also</span></span>

- <span data-ttu-id="c77e1-135">ID のリストからディレクトリ オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="c77e1-135">[Get directory objects from a list of ids](/graph/api/directoryobject-getbyids?view=graph-rest-beta)</span></span>

<!-- uuid: fbec8cd7-cfe4-431d-87fc-d102cd2841a4
2018-12-06 02:01:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryobjectpartnerreference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
