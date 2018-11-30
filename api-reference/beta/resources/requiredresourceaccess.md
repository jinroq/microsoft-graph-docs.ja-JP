---
title: requiredResourceAccess リソースの種類
description: OAuth 2.0 のためのアクセス許可のスコープおよびアプリケーションへのアクセスを必要とする指定したリソース] の下のアプリケーション ロールのセットを指定します。 指定された OAuth 2.0 のアクセス許可の範囲を ( **requiredResourceAccess**コレクション) をクライアント アプリケーションで、要求することがリソースのアプリケーションを呼び出すことです。 アプリケーション エンティティの**requiredResourceAccess**プロパティは、 **ReqiredResourceAccess**のコレクションです。
ms.openlocfilehash: 937557f2f078ade1b336cfd00cd128d428d59cbb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072523"
---
# <a name="requiredresourceaccess-resource-type"></a><span data-ttu-id="b1aa7-105">requiredResourceAccess リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b1aa7-105">requiredResourceAccess resource type</span></span>

> <span data-ttu-id="b1aa7-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b1aa7-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1aa7-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1aa7-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b1aa7-108">OAuth 2.0 のためのアクセス許可のスコープおよびアプリケーションへのアクセスを必要とする指定したリソース] の下のアプリケーション ロールのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="b1aa7-108">Specifies the set of OAuth 2.0 permission scopes and app roles under the specified resource that an application requires access to.</span></span> <span data-ttu-id="b1aa7-109">指定された OAuth 2.0 のアクセス許可の範囲を ( **requiredResourceAccess**コレクション) をクライアント アプリケーションで、要求することがリソースのアプリケーションを呼び出すことです。</span><span class="sxs-lookup"><span data-stu-id="b1aa7-109">The specified OAuth 2.0 permission scopes may be requested by client applications (through the **requiredResourceAccess** collection) when calling a resource application.</span></span> <span data-ttu-id="b1aa7-110">[アプリケーション](application.md)エンティティの**requiredResourceAccess**プロパティは、 **ReqiredResourceAccess**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="b1aa7-110">The **requiredResourceAccess** property of the [application](application.md) entity is a collection of **ReqiredResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b1aa7-111">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b1aa7-111">JSON representation</span></span>

<span data-ttu-id="b1aa7-112">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="b1aa7-112">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requiredResourceAccess"
}-->

```json
{
  "resourceAccess": [{"@odata.type": "microsoft.graph.resourceAccess"}],
  "resourceAppId": "string"
}

```
## <a name="properties"></a><span data-ttu-id="b1aa7-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1aa7-113">Properties</span></span>
| <span data-ttu-id="b1aa7-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1aa7-114">Property</span></span>     | <span data-ttu-id="b1aa7-115">型</span><span class="sxs-lookup"><span data-stu-id="b1aa7-115">Type</span></span>   |<span data-ttu-id="b1aa7-116">説明</span><span class="sxs-lookup"><span data-stu-id="b1aa7-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1aa7-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="b1aa7-117">resourceAccess</span></span>|<span data-ttu-id="b1aa7-118">[ResourceAccess](resourceaccess.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b1aa7-118">[ResourceAccess](resourceaccess.md) collection</span></span>|<span data-ttu-id="b1aa7-119">OAuth2.0 アクセス許可のスコープと、指定したリソースからアプリケーションを必要とするアプリケーション ロールの一覧です。</span><span class="sxs-lookup"><span data-stu-id="b1aa7-119">The list of OAuth2.0 permission scopes and app roles that the application requires from the specified resource.</span></span>|
|<span data-ttu-id="b1aa7-120">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="b1aa7-120">resourceAppId</span></span>|<span data-ttu-id="b1aa7-121">String</span><span class="sxs-lookup"><span data-stu-id="b1aa7-121">String</span></span>|<span data-ttu-id="b1aa7-122">アプリケーションへのアクセスに必要なリソースの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="b1aa7-122">The unique identifier for the resource that the application requires access to.</span></span>  <span data-ttu-id="b1aa7-123">ターゲット リソースのアプリケーションで宣言されている**appId**に等しい場合があります。</span><span class="sxs-lookup"><span data-stu-id="b1aa7-123">This should be equal to the **appId** declared on the target resource application.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
