---
title: auditActivityInitiator リソースの種類
description: アクティビティを開始する resource オブジェクトを識別します。 イニシエーターには、ユーザー、アプリ、またはシステム (アプリとして考えられる) を指定できます。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2f76c071efd10d2d43887bdd5dd04df0d2aa86d5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974228"
---
# <a name="auditactivityinitiator-resource-type"></a><span data-ttu-id="61b9e-104">auditActivityInitiator リソースの種類</span><span class="sxs-lookup"><span data-stu-id="61b9e-104">auditActivityInitiator resource type</span></span>
<span data-ttu-id="61b9e-105">アクティビティを開始する resource オブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="61b9e-105">Identity the resource object that initiates the activity.</span></span> <span data-ttu-id="61b9e-106">イニシエーターには、ユーザー、アプリ、またはシステム (アプリとして考えられる) を指定できます。</span><span class="sxs-lookup"><span data-stu-id="61b9e-106">The initiator can be a user, an app or a system (which is considered as an app)</span></span>



## <a name="properties"></a><span data-ttu-id="61b9e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="61b9e-107">Properties</span></span>
| <span data-ttu-id="61b9e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="61b9e-108">Property</span></span>     | <span data-ttu-id="61b9e-109">型</span><span class="sxs-lookup"><span data-stu-id="61b9e-109">Type</span></span>   |<span data-ttu-id="61b9e-110">説明</span><span class="sxs-lookup"><span data-stu-id="61b9e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61b9e-111">アプリ</span><span class="sxs-lookup"><span data-stu-id="61b9e-111">app</span></span>|[<span data-ttu-id="61b9e-112">appIdentity</span><span class="sxs-lookup"><span data-stu-id="61b9e-112">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="61b9e-113">アクティビティを開始するリソースがアプリの場合、このプロパティは appId、Name、servicePrincipalId、Name などのアプリ関連情報をすべて示します。</span><span class="sxs-lookup"><span data-stu-id="61b9e-113">If the resource initiating the activity is an app, this property indicates all the app related information like appId, Name, servicePrincipalId, Name.</span></span>|
|<span data-ttu-id="61b9e-114">user</span><span class="sxs-lookup"><span data-stu-id="61b9e-114">user</span></span>|[<span data-ttu-id="61b9e-115">userIdentity</span><span class="sxs-lookup"><span data-stu-id="61b9e-115">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="61b9e-116">アクティビティを開始するリソースがユーザーの場合、このプロパティは、userId、Name、UserPrinicpalName など、すべてのユーザー関連情報を示します。</span><span class="sxs-lookup"><span data-stu-id="61b9e-116">If the resource initiating the activity is a user, this property Indicates all the user related information like userId, Name, UserPrinicpalName.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="61b9e-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="61b9e-117">JSON representation</span></span>

<span data-ttu-id="61b9e-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="61b9e-118">Here is a JSON representation of the resource.</span></span>

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
