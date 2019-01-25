---
title: preAuthorizedApplication リソースの種類
description: アプリケーションおよび暗黙の同意を要求されたアクセス許可を表します。 管理者がアプリケーションに同意を提供する必要があります。 preAuthorizedApplications では、ユーザーが要求されたアクセス許可に同意するものは必要ありません。 PreAuthorizedApplications に記載されているアクセス許可では、ユーザーの同意は必要ありません。 ただし、preAuthorizedApplications に記載されていない追加の要求されたアクセス許可は、ユーザーの同意を必要とします。
localization_priority: Normal
ms.openlocfilehash: 22945589341066f4609d47773cb04426774648fd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524549"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="a2ae9-107">preAuthorizedApplication リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a2ae9-107">preAuthorizedApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2ae9-108">アプリケーションおよび暗黙の同意を要求されたアクセス許可を表します。</span><span class="sxs-lookup"><span data-stu-id="a2ae9-108">Represents an application and requested permissions for implicit consent.</span></span> <span data-ttu-id="a2ae9-109">管理者がアプリケーションに同意を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2ae9-109">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="a2ae9-110">preAuthorizedApplications では、ユーザーが要求されたアクセス許可に同意するものは必要ありません。</span><span class="sxs-lookup"><span data-stu-id="a2ae9-110">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="a2ae9-111">PreAuthorizedApplications に記載されているアクセス許可では、ユーザーの同意は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="a2ae9-111">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="a2ae9-112">ただし、preAuthorizedApplications に記載されていない追加の要求されたアクセス許可は、ユーザーの同意を必要とします。</span><span class="sxs-lookup"><span data-stu-id="a2ae9-112">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="a2ae9-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2ae9-113">Properties</span></span>

| <span data-ttu-id="a2ae9-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2ae9-114">Property</span></span> | <span data-ttu-id="a2ae9-115">型</span><span class="sxs-lookup"><span data-stu-id="a2ae9-115">Type</span></span> | <span data-ttu-id="a2ae9-116">説明</span><span class="sxs-lookup"><span data-stu-id="a2ae9-116">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a2ae9-117">appId</span><span class="sxs-lookup"><span data-stu-id="a2ae9-117">appId</span></span>|<span data-ttu-id="a2ae9-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="a2ae9-118">String</span></span>| <span data-ttu-id="a2ae9-119">アプリケーションの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="a2ae9-119">The unique identifier for the application.</span></span> |
|<span data-ttu-id="a2ae9-120">permissionIds</span><span class="sxs-lookup"><span data-stu-id="a2ae9-120">permissionIds</span></span>|<span data-ttu-id="a2ae9-121">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a2ae9-121">String collection</span></span>| <span data-ttu-id="a2ae9-122">[PublishedPermissionScope](permissionscope.md)または[エンティティ](approle.md)は、アプリケーションのいずれかの一意の識別子が必要です。</span><span class="sxs-lookup"><span data-stu-id="a2ae9-122">The unique identifier for either the [publishedPermissionScope](permissionscope.md) or [appRole](approle.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a2ae9-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a2ae9-123">JSON representation</span></span>
<span data-ttu-id="a2ae9-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a2ae9-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.preAuthorizedApplication"
}-->

```json
{
  "appId": "String",
  "permissionIds": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "preAuthorizedApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/preauthorizedapplication.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
