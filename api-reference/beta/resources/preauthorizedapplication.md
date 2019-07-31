---
title: preAuthorizedApplication リソースの種類
description: アプリケーションと、暗黙的同意の要求されたアクセス許可を表します。 管理者はアプリケーションに同意を得る必要があります。 preAuthorizedApplications では、ユーザーが要求されたアクセス許可に同意する必要はありません。 PreAuthorizedApplications にリストされているアクセス許可は、ユーザーの同意を必要としません。 ただし、preAuthorizedApplications に表示されていない追加の要求されたアクセス許可には、ユーザーの同意が必要です。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7adaf4fe960b762b12f6b2cc8607e64c9813712e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965818"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="6042e-107">preAuthorizedApplication リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6042e-107">preAuthorizedApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6042e-108">アプリケーションと、暗黙的同意の要求されたアクセス許可を表します。</span><span class="sxs-lookup"><span data-stu-id="6042e-108">Represents an application and requested permissions for implicit consent.</span></span> <span data-ttu-id="6042e-109">管理者はアプリケーションに同意を得る必要があります。</span><span class="sxs-lookup"><span data-stu-id="6042e-109">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="6042e-110">preAuthorizedApplications では、ユーザーが要求されたアクセス許可に同意する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="6042e-110">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="6042e-111">PreAuthorizedApplications にリストされているアクセス許可は、ユーザーの同意を必要としません。</span><span class="sxs-lookup"><span data-stu-id="6042e-111">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="6042e-112">ただし、preAuthorizedApplications に表示されていない追加の要求されたアクセス許可には、ユーザーの同意が必要です。</span><span class="sxs-lookup"><span data-stu-id="6042e-112">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="6042e-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6042e-113">Properties</span></span>

| <span data-ttu-id="6042e-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6042e-114">Property</span></span> | <span data-ttu-id="6042e-115">型</span><span class="sxs-lookup"><span data-stu-id="6042e-115">Type</span></span> | <span data-ttu-id="6042e-116">説明</span><span class="sxs-lookup"><span data-stu-id="6042e-116">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6042e-117">appId</span><span class="sxs-lookup"><span data-stu-id="6042e-117">appId</span></span>|<span data-ttu-id="6042e-118">String</span><span class="sxs-lookup"><span data-stu-id="6042e-118">String</span></span>| <span data-ttu-id="6042e-119">アプリケーションの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="6042e-119">The unique identifier for the application.</span></span> |
|<span data-ttu-id="6042e-120">permissionIds</span><span class="sxs-lookup"><span data-stu-id="6042e-120">permissionIds</span></span>|<span data-ttu-id="6042e-121">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="6042e-121">String collection</span></span>| <span data-ttu-id="6042e-122">アプリケーションが必要とする[Publishedpermissionscope](permissionscope.md)または[approle](approle.md)の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="6042e-122">The unique identifier for either the [publishedPermissionScope](permissionscope.md) or [appRole](approle.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6042e-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6042e-123">JSON representation</span></span>
<span data-ttu-id="6042e-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6042e-124">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
