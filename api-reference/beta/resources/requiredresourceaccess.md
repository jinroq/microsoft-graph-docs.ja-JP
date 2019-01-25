---
title: requiredResourceAccess リソースの種類
description: OAuth 2.0 のためのアクセス許可のスコープおよびアプリケーションへのアクセスを必要とする指定したリソース] の下のアプリケーション ロールのセットを指定します。 指定された OAuth 2.0 のアクセス許可の範囲を ( **requiredResourceAccess**コレクション) をクライアント アプリケーションで、要求することがリソースのアプリケーションを呼び出すことです。 アプリケーション エンティティの**requiredResourceAccess**プロパティは、 **ReqiredResourceAccess**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: a2c7e337bbe441275f395c2333b8cee918e6b9da
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512970"
---
# <a name="requiredresourceaccess-resource-type"></a><span data-ttu-id="479ac-105">requiredResourceAccess リソースの種類</span><span class="sxs-lookup"><span data-stu-id="479ac-105">requiredResourceAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="479ac-106">OAuth 2.0 のためのアクセス許可のスコープおよびアプリケーションへのアクセスを必要とする指定したリソース] の下のアプリケーション ロールのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="479ac-106">Specifies the set of OAuth 2.0 permission scopes and app roles under the specified resource that an application requires access to.</span></span> <span data-ttu-id="479ac-107">指定された OAuth 2.0 のアクセス許可の範囲を ( **requiredResourceAccess**コレクション) をクライアント アプリケーションで、要求することがリソースのアプリケーションを呼び出すことです。</span><span class="sxs-lookup"><span data-stu-id="479ac-107">The specified OAuth 2.0 permission scopes may be requested by client applications (through the **requiredResourceAccess** collection) when calling a resource application.</span></span> <span data-ttu-id="479ac-108">[アプリケーション](application.md)エンティティの**requiredResourceAccess**プロパティは、 **ReqiredResourceAccess**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="479ac-108">The **requiredResourceAccess** property of the [application](application.md) entity is a collection of **ReqiredResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="479ac-109">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="479ac-109">JSON representation</span></span>

<span data-ttu-id="479ac-110">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="479ac-110">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="479ac-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="479ac-111">Properties</span></span>
| <span data-ttu-id="479ac-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="479ac-112">Property</span></span>     | <span data-ttu-id="479ac-113">型</span><span class="sxs-lookup"><span data-stu-id="479ac-113">Type</span></span>   |<span data-ttu-id="479ac-114">説明</span><span class="sxs-lookup"><span data-stu-id="479ac-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="479ac-115">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="479ac-115">resourceAccess</span></span>|<span data-ttu-id="479ac-116">[ResourceAccess](resourceaccess.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="479ac-116">[ResourceAccess](resourceaccess.md) collection</span></span>|<span data-ttu-id="479ac-117">OAuth2.0 アクセス許可のスコープと、指定したリソースからアプリケーションを必要とするアプリケーション ロールの一覧です。</span><span class="sxs-lookup"><span data-stu-id="479ac-117">The list of OAuth2.0 permission scopes and app roles that the application requires from the specified resource.</span></span>|
|<span data-ttu-id="479ac-118">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="479ac-118">resourceAppId</span></span>|<span data-ttu-id="479ac-119">String</span><span class="sxs-lookup"><span data-stu-id="479ac-119">String</span></span>|<span data-ttu-id="479ac-120">アプリケーションへのアクセスに必要なリソースの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="479ac-120">The unique identifier for the resource that the application requires access to.</span></span>  <span data-ttu-id="479ac-121">ターゲット リソースのアプリケーションで宣言されている**appId**に等しい場合があります。</span><span class="sxs-lookup"><span data-stu-id="479ac-121">This should be equal to the **appId** declared on the target resource application.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/requiredresourceaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
