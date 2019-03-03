---
title: alertHistoryState リソースの種類
description: 通知にパッチが適用されるたびに、変更は alertHistoryState の新しいオブジェクトに保存され、変更された通知の一部として返されます。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: a5dda54101264ee2ec4d01a283f96a93f1d6e5e3
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366967"
---
# <a name="alerthistorystate-resource-type"></a><span data-ttu-id="4c610-103">alertHistoryState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4c610-103">alertHistoryState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c610-104">通知にパッチが適用されるたびに、変更は alertHistoryState の新しいオブジェクトに保存され、変更された通知の一部として返されます。</span><span class="sxs-lookup"><span data-stu-id="4c610-104">Each time an alert is patched, the change is saved in a new object of alertHistoryState, and will be returned as part of the modified alert.</span></span>

## <a name="properties"></a><span data-ttu-id="4c610-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c610-105">Properties</span></span>

| <span data-ttu-id="4c610-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c610-106">Property</span></span>     | <span data-ttu-id="4c610-107">型</span><span class="sxs-lookup"><span data-stu-id="4c610-107">Type</span></span>        | <span data-ttu-id="4c610-108">説明</span><span class="sxs-lookup"><span data-stu-id="4c610-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4c610-109">appId</span><span class="sxs-lookup"><span data-stu-id="4c610-109">appId</span></span>|<span data-ttu-id="4c610-110">String</span><span class="sxs-lookup"><span data-stu-id="4c610-110">String</span></span>| <span data-ttu-id="4c610-111">通知に更新プログラム (パッチ) を送信した、呼び出し元アプリケーションのアプリケーション ID。</span><span class="sxs-lookup"><span data-stu-id="4c610-111">The Application ID of the calling application that submitted an update (PATCH) to the alert.</span></span> <span data-ttu-id="4c610-112">appId は、認証トークンから抽出され、呼び出し元アプリケーションによって手動で入力されることはありません。</span><span class="sxs-lookup"><span data-stu-id="4c610-112">The appId should be extracted from the auth token and not entered manually by the calling application.</span></span> |
|<span data-ttu-id="4c610-113">assignedTo</span><span class="sxs-lookup"><span data-stu-id="4c610-113">assignedTo</span></span>|<span data-ttu-id="4c610-114">String</span><span class="sxs-lookup"><span data-stu-id="4c610-114">String</span></span>| <span data-ttu-id="4c610-115">通知が割り当てられたユーザーの UPN (注: 通知は、最新の値/UPN のみを保存します)。</span><span class="sxs-lookup"><span data-stu-id="4c610-115">UPN of user the alert was assigned to (note: alert.assignedTo only stores the last value/UPN).</span></span> |
|<span data-ttu-id="4c610-116">comments</span><span class="sxs-lookup"><span data-stu-id="4c610-116">comments</span></span>|<span data-ttu-id="4c610-117">String コレクション</span><span class="sxs-lookup"><span data-stu-id="4c610-117">String collection</span></span>|<span data-ttu-id="4c610-118">サインインしているユーザーによって入力されたコメント。</span><span class="sxs-lookup"><span data-stu-id="4c610-118">Comment entered by signed-in user.</span></span>|
|<span data-ttu-id="4c610-119">feedback</span><span class="sxs-lookup"><span data-stu-id="4c610-119">feedback</span></span>|<span data-ttu-id="4c610-120">String</span><span class="sxs-lookup"><span data-stu-id="4c610-120">String</span></span>| <span data-ttu-id="4c610-121">この更新プログラムの通知に関するアナリストからのフィードバック。</span><span class="sxs-lookup"><span data-stu-id="4c610-121">Analyst feedback on the alert in this update.</span></span> <span data-ttu-id="4c610-122">使用可能な値は、`unknown`、`truePositive`、`falsePositive`、`benignPositive` です。</span><span class="sxs-lookup"><span data-stu-id="4c610-122">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="4c610-123">status</span><span class="sxs-lookup"><span data-stu-id="4c610-123">status</span></span>|<span data-ttu-id="4c610-124">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4c610-124">String</span></span>| <span data-ttu-id="4c610-125">警告の状態の値 (更新された場合)。</span><span class="sxs-lookup"><span data-stu-id="4c610-125">Alert status value (if updated).</span></span> <span data-ttu-id="4c610-126">可能な値は、`unknown`、`newAlert`、`inProgress`、`resolved`、`dismissed` です。</span><span class="sxs-lookup"><span data-stu-id="4c610-126">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`.</span></span>|
|<span data-ttu-id="4c610-127">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c610-127">updatedDateTime</span></span>|<span data-ttu-id="4c610-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c610-128">DateTimeOffset</span></span>| <span data-ttu-id="4c610-129">通知の更新日時。</span><span class="sxs-lookup"><span data-stu-id="4c610-129">Date and time of the alert update.</span></span> <span data-ttu-id="4c610-130">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="4c610-130">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4c610-131">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4c610-131">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4c610-132">user</span><span class="sxs-lookup"><span data-stu-id="4c610-132">user</span></span>|<span data-ttu-id="4c610-133">String</span><span class="sxs-lookup"><span data-stu-id="4c610-133">String</span></span>| <span data-ttu-id="4c610-134">アラートを更新したサインインしているユーザーの UPN (ユーザー/委任された認証モードの場合は、ベアラートークンから取得)。</span><span class="sxs-lookup"><span data-stu-id="4c610-134">UPN of the signed-in user that updated the alert (taken from the bearer token - if in user/delegated auth mode).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4c610-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4c610-135">JSON representation</span></span>

<span data-ttu-id="4c610-136">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4c610-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertHistoryState",
  "baseType": null
}-->

```json
{
  "appId": "String",
  "assignedTo": "String",
  "comments": ["String"],
  "feedback": "String",
  "status": "String",
  "updatedDateTime": "String (timestamp)",
  "user": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertHistoryState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->