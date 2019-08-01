---
title: directoryObjectPartnerReference リソースの種類
description: パートナーテナント内のディレクトリオブジェクトへの参照を表します。 directoryObject から継承します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7b8fb49ac74d7f1a603f5f0b74d47751242ae01a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029471"
---
# <a name="directoryobjectpartnerreference-resource-type"></a><span data-ttu-id="baa5e-104">directoryObjectPartnerReference リソースの種類</span><span class="sxs-lookup"><span data-stu-id="baa5e-104">directoryObjectPartnerReference resource type</span></span>

<span data-ttu-id="baa5e-105">パートナー組織内のディレクトリオブジェクトへの参照を表します。</span><span class="sxs-lookup"><span data-stu-id="baa5e-105">Represents a reference to a directory object in a partner organization.</span></span> <span data-ttu-id="baa5e-106">[directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) から継承します。</span><span class="sxs-lookup"><span data-stu-id="baa5e-106">Inherits from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span></span>

## <a name="properties"></a><span data-ttu-id="baa5e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="baa5e-107">Properties</span></span>

| <span data-ttu-id="baa5e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="baa5e-108">Property</span></span> | <span data-ttu-id="baa5e-109">型</span><span class="sxs-lookup"><span data-stu-id="baa5e-109">Type</span></span> | <span data-ttu-id="baa5e-110">説明</span><span class="sxs-lookup"><span data-stu-id="baa5e-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="baa5e-111">description</span><span class="sxs-lookup"><span data-stu-id="baa5e-111">description</span></span>|<span data-ttu-id="baa5e-112">String</span><span class="sxs-lookup"><span data-stu-id="baa5e-112">String</span></span>| <span data-ttu-id="baa5e-113">返されるオブジェクトの説明。</span><span class="sxs-lookup"><span data-stu-id="baa5e-113">Description of the object returned.</span></span> <span data-ttu-id="baa5e-114">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="baa5e-114">Read-only.</span></span> |
|<span data-ttu-id="baa5e-115">displayName</span><span class="sxs-lookup"><span data-stu-id="baa5e-115">displayName</span></span>|<span data-ttu-id="baa5e-116">String</span><span class="sxs-lookup"><span data-stu-id="baa5e-116">String</span></span>| <span data-ttu-id="baa5e-117">グループまたはアプリケーションなど、返されるディレクトリオブジェクトの名前。</span><span class="sxs-lookup"><span data-stu-id="baa5e-117">Name of directory object being returned, like group or application.</span></span> <span data-ttu-id="baa5e-118">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="baa5e-118">Read-only.</span></span> |
|<span data-ttu-id="baa5e-119">externalPartnerTenantId</span><span class="sxs-lookup"><span data-stu-id="baa5e-119">externalPartnerTenantId</span></span>|<span data-ttu-id="baa5e-120">Guid</span><span class="sxs-lookup"><span data-stu-id="baa5e-120">Guid</span></span>| <span data-ttu-id="baa5e-121">パートナーテナントのテナント識別子。</span><span class="sxs-lookup"><span data-stu-id="baa5e-121">The tenant identifier for the partner tenant.</span></span> <span data-ttu-id="baa5e-122">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="baa5e-122">Read-only.</span></span> |
|<span data-ttu-id="baa5e-123">id</span><span class="sxs-lookup"><span data-stu-id="baa5e-123">id</span></span>|<span data-ttu-id="baa5e-124">文字列</span><span class="sxs-lookup"><span data-stu-id="baa5e-124">String</span></span>| <span data-ttu-id="baa5e-125">リソースの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="baa5e-125">The unique identifier for the resource.</span></span> <span data-ttu-id="baa5e-126">[directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) から継承されます。</span><span class="sxs-lookup"><span data-stu-id="baa5e-126">Inherited from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).</span></span> <span data-ttu-id="baa5e-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="baa5e-127">Read-only.</span></span> |
|<span data-ttu-id="baa5e-128">objectType</span><span class="sxs-lookup"><span data-stu-id="baa5e-128">objectType</span></span>|<span data-ttu-id="baa5e-129">文字列</span><span class="sxs-lookup"><span data-stu-id="baa5e-129">String</span></span>| <span data-ttu-id="baa5e-130">パートナーテナント内の参照されるオブジェクトの種類。</span><span class="sxs-lookup"><span data-stu-id="baa5e-130">The type of the referenced object in the partner tenant.</span></span> <span data-ttu-id="baa5e-131">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="baa5e-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="baa5e-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="baa5e-132">JSON representation</span></span>

<span data-ttu-id="baa5e-133">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="baa5e-133">The following is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="baa5e-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="baa5e-134">See also</span></span>

- [<span data-ttu-id="baa5e-135">ID のリストからディレクトリ オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="baa5e-135">Get directory objects from a list of ids</span></span>](/graph/api/directoryobject-getbyids?view=graph-rest-v1.0)

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
