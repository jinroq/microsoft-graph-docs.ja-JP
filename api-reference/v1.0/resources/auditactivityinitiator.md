---
title: auditActivityInitiator リソースの種類
description: アクティビティを開始する resource オブジェクトを識別します。 イニシエーターには、ユーザー、アプリ、またはシステム (アプリとして認識される) を指定できます。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d5de4cc65379a3386137c7da79a10c5492dd1427
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629349"
---
# <a name="auditactivityinitiator-resource-type"></a><span data-ttu-id="1fe94-104">auditActivityInitiator リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1fe94-104">auditActivityInitiator resource type</span></span>

<span data-ttu-id="1fe94-105">アクティビティを開始する resource オブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="1fe94-105">Identity the resource object that initiates the activity.</span></span> <span data-ttu-id="1fe94-106">イニシエーターには、ユーザー、アプリ、またはシステム (アプリと見なされる) を使用できます。</span><span class="sxs-lookup"><span data-stu-id="1fe94-106">The initiator can be a user, an app, or a system (which is considered an app).</span></span>

## <a name="properties"></a><span data-ttu-id="1fe94-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1fe94-107">Properties</span></span>

| <span data-ttu-id="1fe94-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1fe94-108">Property</span></span>     | <span data-ttu-id="1fe94-109">型</span><span class="sxs-lookup"><span data-stu-id="1fe94-109">Type</span></span>   |<span data-ttu-id="1fe94-110">説明</span><span class="sxs-lookup"><span data-stu-id="1fe94-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1fe94-111">アプリ</span><span class="sxs-lookup"><span data-stu-id="1fe94-111">app</span></span>|[<span data-ttu-id="1fe94-112">appIdentity</span><span class="sxs-lookup"><span data-stu-id="1fe94-112">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="1fe94-113">アクティビティを開始するリソースがアプリの場合、このプロパティは appId、Name、servicePrincipalId、Name などのアプリ関連情報をすべて示します。</span><span class="sxs-lookup"><span data-stu-id="1fe94-113">If the resource initiating the activity is an app, this property indicates all the app related information like appId, Name, servicePrincipalId, Name.</span></span>|
|<span data-ttu-id="1fe94-114">user</span><span class="sxs-lookup"><span data-stu-id="1fe94-114">user</span></span>|[<span data-ttu-id="1fe94-115">userIdentity</span><span class="sxs-lookup"><span data-stu-id="1fe94-115">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="1fe94-116">アクティビティを開始するリソースがユーザーの場合、このプロパティは、userId、Name、UserPrinicpalName など、すべてのユーザー関連情報を示します。</span><span class="sxs-lookup"><span data-stu-id="1fe94-116">If the resource initiating the activity is a user, this property Indicates all the user related information like userId, Name, UserPrinicpalName.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1fe94-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1fe94-117">JSON representation</span></span>

<span data-ttu-id="1fe94-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1fe94-118">Here is a JSON representation of the resource.</span></span>

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
