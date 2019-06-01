---
title: applicationSignInDetailedSummary リソースの種類-Microsoft Graph API
description: アプリケーションサインインの詳細な概要を表します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4d4fcd00e305c19f1d445738a22125cc8addc143
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657638"
---
# <a name="applicationsignindetailedsummary-resource-type"></a><span data-ttu-id="dfdd6-103">applicationSignInDetailedSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dfdd6-103">applicationSignInDetailedSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfdd6-104">アプリケーションサインインの詳細な概要を表します。</span><span class="sxs-lookup"><span data-stu-id="dfdd6-104">Represents a detailed summary of an application sign-in.</span></span>

## <a name="methods"></a><span data-ttu-id="dfdd6-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="dfdd6-105">Methods</span></span>

| <span data-ttu-id="dfdd6-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="dfdd6-106">Method</span></span>       | <span data-ttu-id="dfdd6-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="dfdd6-107">Return Type</span></span> | <span data-ttu-id="dfdd6-108">説明</span><span class="sxs-lookup"><span data-stu-id="dfdd6-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="dfdd6-109">ApplicationSignInDetailedSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="dfdd6-109">Get applicationSignInDetailedSummary</span></span>](../api/applicationsignindetailedsummary-get.md) | [<span data-ttu-id="dfdd6-110">applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="dfdd6-110">applicationSignInDetailedSummary</span></span>](applicationsignindetailedsummary.md) | <span data-ttu-id="dfdd6-111">**ApplicationSignInDetailedSummary**オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="dfdd6-111">Read the properties and relationships of an **applicationSignInDetailedSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="dfdd6-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfdd6-112">Properties</span></span>
| <span data-ttu-id="dfdd6-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfdd6-113">Property</span></span>     | <span data-ttu-id="dfdd6-114">型</span><span class="sxs-lookup"><span data-stu-id="dfdd6-114">Type</span></span>        | <span data-ttu-id="dfdd6-115">説明</span><span class="sxs-lookup"><span data-stu-id="dfdd6-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dfdd6-116">aggregatedEventDateTime</span><span class="sxs-lookup"><span data-stu-id="dfdd6-116">aggregatedEventDateTime</span></span>|<span data-ttu-id="dfdd6-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfdd6-117">DateTimeOffset</span></span>|<span data-ttu-id="dfdd6-118">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="dfdd6-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="dfdd6-119">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="dfdd6-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="dfdd6-120">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="dfdd6-120">appDisplayName</span></span>|<span data-ttu-id="dfdd6-121">String</span><span class="sxs-lookup"><span data-stu-id="dfdd6-121">String</span></span>|<span data-ttu-id="dfdd6-122">ユーザーがサインインしたアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="dfdd6-122">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="dfdd6-123">appId</span><span class="sxs-lookup"><span data-stu-id="dfdd6-123">appId</span></span>|<span data-ttu-id="dfdd6-124">String</span><span class="sxs-lookup"><span data-stu-id="dfdd6-124">String</span></span>|<span data-ttu-id="dfdd6-125">ユーザーがサインインしたアプリケーションの ID。</span><span class="sxs-lookup"><span data-stu-id="dfdd6-125">ID of the application that the user signed in to.</span></span>|
|<span data-ttu-id="dfdd6-126">id</span><span class="sxs-lookup"><span data-stu-id="dfdd6-126">id</span></span>|<span data-ttu-id="dfdd6-127">文字列</span><span class="sxs-lookup"><span data-stu-id="dfdd6-127">String</span></span>| <span data-ttu-id="dfdd6-128">サインインアクティビティを表す一意の ID。</span><span class="sxs-lookup"><span data-stu-id="dfdd6-128">A unique ID representing the sign-in activity.</span></span>|
|<span data-ttu-id="dfdd6-129">signInCount</span><span class="sxs-lookup"><span data-stu-id="dfdd6-129">signInCount</span></span>|<span data-ttu-id="dfdd6-130">Int64</span><span class="sxs-lookup"><span data-stu-id="dfdd6-130">Int64</span></span>|<span data-ttu-id="dfdd6-131">アプリケーションによって作成されたサインインの数。</span><span class="sxs-lookup"><span data-stu-id="dfdd6-131">Count of sign-ins made by the application.</span></span>|
|<span data-ttu-id="dfdd6-132">status</span><span class="sxs-lookup"><span data-stu-id="dfdd6-132">status</span></span>|[<span data-ttu-id="dfdd6-133">signInStatus</span><span class="sxs-lookup"><span data-stu-id="dfdd6-133">signInStatus</span></span>](signinstatus.md)|<span data-ttu-id="dfdd6-134">サインイン状態の詳細。</span><span class="sxs-lookup"><span data-stu-id="dfdd6-134">Details of the sign-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfdd6-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dfdd6-135">Relationships</span></span>
<span data-ttu-id="dfdd6-136">なし</span><span class="sxs-lookup"><span data-stu-id="dfdd6-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="dfdd6-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dfdd6-137">JSON representation</span></span>

<span data-ttu-id="dfdd6-138">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dfdd6-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationSignInDetailedSummary"
}-->

```json
{
  "aggregatedEventDateTime": "String (timestamp)",
  "appDisplayName": "String",
  "appId": "String",
  "id": "String (identifier)",
  "signInCount": 1024,
  "status": {"@odata.type": "microsoft.graph.signInStatus"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationSignInDetailedSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
