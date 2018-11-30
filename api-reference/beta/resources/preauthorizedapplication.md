---
title: preAuthorizedApplication リソースの種類
description: アプリケーションおよび暗黙の同意を要求されたアクセス許可を表します。 管理者がアプリケーションに同意を提供する必要があります。 preAuthorizedApplications では、ユーザーが要求されたアクセス許可に同意するものは必要ありません。 PreAuthorizedApplications に記載されているアクセス許可では、ユーザーの同意は必要ありません。 ただし、preAuthorizedApplications に記載されていない追加の要求されたアクセス許可は、ユーザーの同意を必要とします。
ms.openlocfilehash: d299aefcac541407e0e42d0b0933e903afa3e84d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074094"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="5904d-107">preAuthorizedApplication リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5904d-107">preAuthorizedApplication resource type</span></span>

> <span data-ttu-id="5904d-108">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5904d-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5904d-109">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5904d-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5904d-110">アプリケーションおよび暗黙の同意を要求されたアクセス許可を表します。</span><span class="sxs-lookup"><span data-stu-id="5904d-110">Represents an application and requested permissions for implicit consent.</span></span> <span data-ttu-id="5904d-111">管理者がアプリケーションに同意を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5904d-111">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="5904d-112">preAuthorizedApplications では、ユーザーが要求されたアクセス許可に同意するものは必要ありません。</span><span class="sxs-lookup"><span data-stu-id="5904d-112">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="5904d-113">PreAuthorizedApplications に記載されているアクセス許可では、ユーザーの同意は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="5904d-113">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="5904d-114">ただし、preAuthorizedApplications に記載されていない追加の要求されたアクセス許可は、ユーザーの同意を必要とします。</span><span class="sxs-lookup"><span data-stu-id="5904d-114">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="5904d-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5904d-115">Properties</span></span>

| <span data-ttu-id="5904d-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5904d-116">Property</span></span> | <span data-ttu-id="5904d-117">型</span><span class="sxs-lookup"><span data-stu-id="5904d-117">Type</span></span> | <span data-ttu-id="5904d-118">説明</span><span class="sxs-lookup"><span data-stu-id="5904d-118">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="5904d-119">appId</span><span class="sxs-lookup"><span data-stu-id="5904d-119">appId</span></span>|<span data-ttu-id="5904d-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="5904d-120">String</span></span>| <span data-ttu-id="5904d-121">アプリケーションの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="5904d-121">The unique identifier for the application.</span></span> |
|<span data-ttu-id="5904d-122">permissionIds</span><span class="sxs-lookup"><span data-stu-id="5904d-122">permissionIds</span></span>|<span data-ttu-id="5904d-123">String コレクション</span><span class="sxs-lookup"><span data-stu-id="5904d-123">String collection</span></span>| <span data-ttu-id="5904d-124">[PublishedPermissionScope](permissionscope.md)または[エンティティ](approle.md)は、アプリケーションのいずれかの一意の識別子が必要です。</span><span class="sxs-lookup"><span data-stu-id="5904d-124">The unique identifier for either the [publishedPermissionScope](permissionscope.md) or [appRole](approle.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5904d-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5904d-125">JSON representation</span></span>
<span data-ttu-id="5904d-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5904d-126">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "preAuthorizedApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->