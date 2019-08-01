---
title: userIdentity リソースの種類
description: Azure AD 監査ログのコンテキストでは、これは監査アクティビティの開始または影響を受けたユーザー情報を表します。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0e72f5338f7281188b7023aed342dd34ee57595e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033503"
---
# <a name="useridentity-resource-type"></a><span data-ttu-id="199ff-103">userIdentity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="199ff-103">userIdentity resource type</span></span>

<span data-ttu-id="199ff-104">Azure AD 監査ログのコンテキストでは、これは監査アクティビティの開始または影響を受けたユーザー情報を表します。</span><span class="sxs-lookup"><span data-stu-id="199ff-104">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

## <a name="properties"></a><span data-ttu-id="199ff-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="199ff-105">Properties</span></span>

| <span data-ttu-id="199ff-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="199ff-106">Property</span></span>     | <span data-ttu-id="199ff-107">型</span><span class="sxs-lookup"><span data-stu-id="199ff-107">Type</span></span>   |<span data-ttu-id="199ff-108">説明</span><span class="sxs-lookup"><span data-stu-id="199ff-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="199ff-109">displayName</span><span class="sxs-lookup"><span data-stu-id="199ff-109">displayName</span></span> | <span data-ttu-id="199ff-110">String</span><span class="sxs-lookup"><span data-stu-id="199ff-110">String</span></span> | <span data-ttu-id="199ff-111">Id の表示名。</span><span class="sxs-lookup"><span data-stu-id="199ff-111">The identity's display name.</span></span> <span data-ttu-id="199ff-112">これは、常に有効であったり、最新ではない場合があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="199ff-112">Note that this may not always be available or up-to-date.</span></span>    |
| <span data-ttu-id="199ff-113">id</span><span class="sxs-lookup"><span data-stu-id="199ff-113">id</span></span>          | <span data-ttu-id="199ff-114">文字列</span><span class="sxs-lookup"><span data-stu-id="199ff-114">String</span></span> | <span data-ttu-id="199ff-115">ID の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="199ff-115">Unique identifier for the identity.</span></span>  |
| <span data-ttu-id="199ff-116">ipAddress</span><span class="sxs-lookup"><span data-stu-id="199ff-116">ipAddress</span></span>   | <span data-ttu-id="199ff-117">String</span><span class="sxs-lookup"><span data-stu-id="199ff-117">String</span></span>| <span data-ttu-id="199ff-118">ユーザーがアクティビティを実行するときに使用するクライアント IP アドレスを示します (監査ログのみ)。</span><span class="sxs-lookup"><span data-stu-id="199ff-118">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| <span data-ttu-id="199ff-119">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="199ff-119">userPrincipalName</span></span> | <span data-ttu-id="199ff-120">String</span><span class="sxs-lookup"><span data-stu-id="199ff-120">String</span></span>  | <span data-ttu-id="199ff-121">ユーザーの userPrincipalName 属性。</span><span class="sxs-lookup"><span data-stu-id="199ff-121">The userPrincipalName attribute of the user.</span></span> |

><span data-ttu-id="199ff-122">**注:** 場合によっては、一意の識別子を使用できないことがあります。</span><span class="sxs-lookup"><span data-stu-id="199ff-122">**Note:** In some cases, the unique identifier might not be available.</span></span> <span data-ttu-id="199ff-123">その場合、ID の **displayName** プロパティが返されますが、**id** プロパティはリソースから失われます。</span><span class="sxs-lookup"><span data-stu-id="199ff-123">In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="199ff-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="199ff-124">JSON representation</span></span>

<span data-ttu-id="199ff-125">この型の JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="199ff-125">Here is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
"displayName", "thumbnails"
  ],
  "@odata.type": "microsoft.graph.userIdentity"
}-->

```json
{
  "displayName": "string",
  "id": "string",
  "ipAddress": "string",
  "userPrincipalName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/useridentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
