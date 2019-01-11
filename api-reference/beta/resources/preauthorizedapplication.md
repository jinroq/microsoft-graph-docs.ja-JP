---
title: preAuthorizedApplication リソースの種類
description: アプリケーションおよび暗黙の同意を要求されたアクセス許可を表します。 管理者がアプリケーションに同意を提供する必要があります。 preAuthorizedApplications では、ユーザーが要求されたアクセス許可に同意するものは必要ありません。 PreAuthorizedApplications に記載されているアクセス許可では、ユーザーの同意は必要ありません。 ただし、preAuthorizedApplications に記載されていない追加の要求されたアクセス許可は、ユーザーの同意を必要とします。
localization_priority: Normal
ms.openlocfilehash: fa26b8046b81db70300b8ff40abcbd2b84f3f0c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832796"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="d96d5-107">preAuthorizedApplication リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d96d5-107">preAuthorizedApplication resource type</span></span>

> <span data-ttu-id="d96d5-108">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d96d5-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d96d5-109">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d96d5-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d96d5-110">アプリケーションおよび暗黙の同意を要求されたアクセス許可を表します。</span><span class="sxs-lookup"><span data-stu-id="d96d5-110">Represents an application and requested permissions for implicit consent.</span></span> <span data-ttu-id="d96d5-111">管理者がアプリケーションに同意を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d96d5-111">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="d96d5-112">preAuthorizedApplications では、ユーザーが要求されたアクセス許可に同意するものは必要ありません。</span><span class="sxs-lookup"><span data-stu-id="d96d5-112">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="d96d5-113">PreAuthorizedApplications に記載されているアクセス許可では、ユーザーの同意は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="d96d5-113">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="d96d5-114">ただし、preAuthorizedApplications に記載されていない追加の要求されたアクセス許可は、ユーザーの同意を必要とします。</span><span class="sxs-lookup"><span data-stu-id="d96d5-114">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="d96d5-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d96d5-115">Properties</span></span>

| <span data-ttu-id="d96d5-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d96d5-116">Property</span></span> | <span data-ttu-id="d96d5-117">種類</span><span class="sxs-lookup"><span data-stu-id="d96d5-117">Type</span></span> | <span data-ttu-id="d96d5-118">説明</span><span class="sxs-lookup"><span data-stu-id="d96d5-118">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d96d5-119">appId</span><span class="sxs-lookup"><span data-stu-id="d96d5-119">appId</span></span>|<span data-ttu-id="d96d5-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d96d5-120">String</span></span>| <span data-ttu-id="d96d5-121">アプリケーションの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="d96d5-121">The unique identifier for the application.</span></span> |
|<span data-ttu-id="d96d5-122">permissionIds</span><span class="sxs-lookup"><span data-stu-id="d96d5-122">permissionIds</span></span>|<span data-ttu-id="d96d5-123">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d96d5-123">String collection</span></span>| <span data-ttu-id="d96d5-124">[PublishedPermissionScope](permissionscope.md)または[エンティティ](approle.md)は、アプリケーションのいずれかの一意の識別子が必要です。</span><span class="sxs-lookup"><span data-stu-id="d96d5-124">The unique identifier for either the [publishedPermissionScope](permissionscope.md) or [appRole](approle.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d96d5-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d96d5-125">JSON representation</span></span>
<span data-ttu-id="d96d5-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d96d5-126">Here is a JSON representation of the resource.</span></span>

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
