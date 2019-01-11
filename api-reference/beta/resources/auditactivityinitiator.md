---
title: auditActivityInitiator リソースの種類
description: 活動を開始するリソース オブジェクトの id。 ユーザー、アプリケーションまたはシステム (これはアプリケーションとしてと見なされます) をイニシエーターとして使用することができます。
localization_priority: Normal
ms.openlocfilehash: 14c92a4df42c3d8dbcd6836695df8d6caac3cf87
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884610"
---
# <a name="auditactivityinitiator-resource-type"></a><span data-ttu-id="3ab91-104">auditActivityInitiator リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3ab91-104">auditActivityInitiator resource type</span></span>
<span data-ttu-id="3ab91-105">活動を開始するリソース オブジェクトの id。</span><span class="sxs-lookup"><span data-stu-id="3ab91-105">Identity the resource object that initiates the activity.</span></span> <span data-ttu-id="3ab91-106">ユーザー、アプリケーションまたはシステム (これはアプリケーションとしてと見なされます) をイニシエーターとして使用することができます。</span><span class="sxs-lookup"><span data-stu-id="3ab91-106">The initiator can be a user, an app or a system (which is considered as an app)</span></span>



## <a name="properties"></a><span data-ttu-id="3ab91-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ab91-107">Properties</span></span>
| <span data-ttu-id="3ab91-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ab91-108">Property</span></span>     | <span data-ttu-id="3ab91-109">種類</span><span class="sxs-lookup"><span data-stu-id="3ab91-109">Type</span></span>   |<span data-ttu-id="3ab91-110">説明</span><span class="sxs-lookup"><span data-stu-id="3ab91-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ab91-111">アプリ</span><span class="sxs-lookup"><span data-stu-id="3ab91-111">app</span></span>|[<span data-ttu-id="3ab91-112">appIdentity</span><span class="sxs-lookup"><span data-stu-id="3ab91-112">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="3ab91-113">活動を開始するリソースがアプリケーションの場合は、このプロパティは、すべてのアプリケーションを示します appId などの情報を関連する名前、servicePrincipalId、名前です。</span><span class="sxs-lookup"><span data-stu-id="3ab91-113">If the resource initiating the activity is an app, this property indicates all the app related information like appId, Name, servicePrincipalId, Name.</span></span>|
|<span data-ttu-id="3ab91-114">user</span><span class="sxs-lookup"><span data-stu-id="3ab91-114">user</span></span>|[<span data-ttu-id="3ab91-115">割り当てられていません</span><span class="sxs-lookup"><span data-stu-id="3ab91-115">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="3ab91-116">活動を開始するリソースがユーザーの場合は、このプロパティは、すべてのユーザーを示しますに関連するユーザー Id、名前、UserPrinicpalName のような情報です。</span><span class="sxs-lookup"><span data-stu-id="3ab91-116">If the resource initiating the activity is a user, this property Indicates all the user related information like userId, Name, UserPrinicpalName.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3ab91-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3ab91-117">JSON representation</span></span>

<span data-ttu-id="3ab91-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3ab91-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.auditActivityInitiator"
}-->

```json
{
  "app": {"@odata.type": "microsoft.graph.appIdentity"},
  "user": {"@odata.type": "microsoft.graph.userIdentity"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "auditActivityInitiator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
