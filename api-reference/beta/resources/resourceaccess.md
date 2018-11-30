---
title: resourceAccess リソースの種類
description: OAuth 2.0 のためのアクセス許可のスコープまたはアプリケーションを必要とするアプリケーションの役割を指定します。 RequiredResourceAccess 型の**resourceAccess**プロパティは、 **ResourceAccess**のコレクションです。
ms.openlocfilehash: 56e9b2b006d63d2a9abebc9e9585744b08438800
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071867"
---
# <a name="resourceaccess-resource-type"></a><span data-ttu-id="330d1-104">resourceAccess リソースの種類</span><span class="sxs-lookup"><span data-stu-id="330d1-104">resourceAccess resource type</span></span>

> <span data-ttu-id="330d1-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="330d1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="330d1-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="330d1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="330d1-107">OAuth 2.0 のためのアクセス許可のスコープまたはアプリケーションを必要とするアプリケーションの役割を指定します。</span><span class="sxs-lookup"><span data-stu-id="330d1-107">Specifies an OAuth 2.0 permission scope or an app role that an application requires.</span></span> <span data-ttu-id="330d1-108">[RequiredResourceAccess](requiredresourceaccess.md)型の**resourceAccess**プロパティは、 **ResourceAccess**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="330d1-108">The **resourceAccess** property of the [requiredResourceAccess](requiredresourceaccess.md) type is a collection of **ResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="330d1-109">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="330d1-109">JSON representation</span></span>

<span data-ttu-id="330d1-110">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="330d1-110">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resourceAccess"
}-->

```json
{
  "id": "guid",
  "type": "string"
}

```
## <a name="properties"></a><span data-ttu-id="330d1-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="330d1-111">Properties</span></span>
| <span data-ttu-id="330d1-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="330d1-112">Property</span></span>     | <span data-ttu-id="330d1-113">型</span><span class="sxs-lookup"><span data-stu-id="330d1-113">Type</span></span>   |<span data-ttu-id="330d1-114">説明</span><span class="sxs-lookup"><span data-stu-id="330d1-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="330d1-115">ID</span><span class="sxs-lookup"><span data-stu-id="330d1-115">id</span></span>|<span data-ttu-id="330d1-116">Guid</span><span class="sxs-lookup"><span data-stu-id="330d1-116">Guid</span></span>|<span data-ttu-id="330d1-117">リソースのアプリケーションを公開する[oAuth2Permission](oauth2permission.md)または[エンティティ](approle.md)のインスタンスの 1 つの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="330d1-117">The unique identifier for one of the [oAuth2Permission](oauth2permission.md) or [appRole](approle.md) instances that the resource application exposes.</span></span>|
|<span data-ttu-id="330d1-118">type</span><span class="sxs-lookup"><span data-stu-id="330d1-118">type</span></span>|<span data-ttu-id="330d1-119">String</span><span class="sxs-lookup"><span data-stu-id="330d1-119">String</span></span>|<span data-ttu-id="330d1-120">[OAuth2Permission](oauth2permission.md)または[エンティティ](approle.md)の**id**プロパティを参照するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="330d1-120">Specifies whether the **id** property references an [oAuth2Permission](oauth2permission.md) or an [appRole](approle.md).</span></span> <span data-ttu-id="330d1-121">使用可能な値は、「スコープ」または「ロール」です。</span><span class="sxs-lookup"><span data-stu-id="330d1-121">Possible values are "scope" or "role".</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
