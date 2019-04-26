---
title: requiredresourceaccess リソースの種類
description: アプリケーションがアクセスを必要とする、指定されたリソースの下にある OAuth 2.0 アクセス許可スコープおよびアプリロールのセットを指定します。 指定された OAuth 2.0 アクセス許可のスコープは、リソースアプリケーションを呼び出すときに、( **requiredresourceaccess**コレクションを通じて) クライアントアプリケーションによって要求されることがあります。 application エンティティの**requiredresourceaccess**プロパティは、 **ReqiredResourceAccess**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: a2c7e337bbe441275f395c2333b8cee918e6b9da
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563176"
---
# <a name="requiredresourceaccess-resource-type"></a><span data-ttu-id="6c0de-105">requiredresourceaccess リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6c0de-105">requiredResourceAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c0de-106">アプリケーションがアクセスを必要とする、指定されたリソースの下にある OAuth 2.0 アクセス許可スコープおよびアプリロールのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="6c0de-106">Specifies the set of OAuth 2.0 permission scopes and app roles under the specified resource that an application requires access to.</span></span> <span data-ttu-id="6c0de-107">指定された OAuth 2.0 アクセス許可のスコープは、リソースアプリケーションを呼び出すときに、( **requiredresourceaccess**コレクションを通じて) クライアントアプリケーションによって要求されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6c0de-107">The specified OAuth 2.0 permission scopes may be requested by client applications (through the **requiredResourceAccess** collection) when calling a resource application.</span></span> <span data-ttu-id="6c0de-108">[application](application.md)エンティティの**requiredresourceaccess**プロパティは、 **ReqiredResourceAccess**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="6c0de-108">The **requiredResourceAccess** property of the [application](application.md) entity is a collection of **ReqiredResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="6c0de-109">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6c0de-109">JSON representation</span></span>

<span data-ttu-id="6c0de-110">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="6c0de-110">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="6c0de-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c0de-111">Properties</span></span>
| <span data-ttu-id="6c0de-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c0de-112">Property</span></span>     | <span data-ttu-id="6c0de-113">型</span><span class="sxs-lookup"><span data-stu-id="6c0de-113">Type</span></span>   |<span data-ttu-id="6c0de-114">説明</span><span class="sxs-lookup"><span data-stu-id="6c0de-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c0de-115">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="6c0de-115">resourceAccess</span></span>|<span data-ttu-id="6c0de-116">[resourceaccess](resourceaccess.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6c0de-116">[ResourceAccess](resourceaccess.md) collection</span></span>|<span data-ttu-id="6c0de-117">指定されたリソースからアプリケーションが必要とする oauth 2.0 のアクセス許可スコープとアプリの役割の一覧。</span><span class="sxs-lookup"><span data-stu-id="6c0de-117">The list of OAuth2.0 permission scopes and app roles that the application requires from the specified resource.</span></span>|
|<span data-ttu-id="6c0de-118">resourceappid</span><span class="sxs-lookup"><span data-stu-id="6c0de-118">resourceAppId</span></span>|<span data-ttu-id="6c0de-119">String</span><span class="sxs-lookup"><span data-stu-id="6c0de-119">String</span></span>|<span data-ttu-id="6c0de-120">アプリケーションがアクセスする必要があるリソースの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="6c0de-120">The unique identifier for the resource that the application requires access to.</span></span>  <span data-ttu-id="6c0de-121">これは、ターゲットリソースアプリケーションで宣言されている**appId**と同じである必要があります。</span><span class="sxs-lookup"><span data-stu-id="6c0de-121">This should be equal to the **appId** declared on the target resource application.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
