---
title: logonUser のリソースの種類
description: このホスト上のログオン中のユーザーに関するステートフルな情報が含まれています
ms.openlocfilehash: 80ff69453e99f5cd5103f85cd7d8c45696057f7c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073458"
---
# <a name="logonuser-resource-type"></a><span data-ttu-id="569f2-103">logonUser のリソースの種類</span><span class="sxs-lookup"><span data-stu-id="569f2-103">logonUser resource type</span></span>

<span data-ttu-id="569f2-104">このホスト上のログオン中のユーザーに関するステートフルな情報が含まれています</span><span class="sxs-lookup"><span data-stu-id="569f2-104">Contains stateful information about the logged on user on this host</span></span>

## <a name="properties"></a><span data-ttu-id="569f2-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="569f2-105">Properties</span></span>

| <span data-ttu-id="569f2-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="569f2-106">Property</span></span>   | <span data-ttu-id="569f2-107">型</span><span class="sxs-lookup"><span data-stu-id="569f2-107">Type</span></span> |<span data-ttu-id="569f2-108">説明</span><span class="sxs-lookup"><span data-stu-id="569f2-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="569f2-109">accountDomain</span><span class="sxs-lookup"><span data-stu-id="569f2-109">accountDomain</span></span>|<span data-ttu-id="569f2-110">String</span><span class="sxs-lookup"><span data-stu-id="569f2-110">String</span></span>|<span data-ttu-id="569f2-111">使用するユーザー アカウントのドメインにログオンします。</span><span class="sxs-lookup"><span data-stu-id="569f2-111">Domain of user account used to logon.</span></span>|
|<span data-ttu-id="569f2-112">accountName</span><span class="sxs-lookup"><span data-stu-id="569f2-112">accountName</span></span>|<span data-ttu-id="569f2-113">String</span><span class="sxs-lookup"><span data-stu-id="569f2-113">String</span></span>|<span data-ttu-id="569f2-114">使用するユーザー アカウントのアカウント名をログオンします。</span><span class="sxs-lookup"><span data-stu-id="569f2-114">Account name of user account used to logon.</span></span>|
|<span data-ttu-id="569f2-115">accountType</span><span class="sxs-lookup"><span data-stu-id="569f2-115">accountType</span></span>|<span data-ttu-id="569f2-116">String</span><span class="sxs-lookup"><span data-stu-id="569f2-116">String</span></span>|<span data-ttu-id="569f2-117">ユーザー アカウントの種類、Windows の定義ごと。</span><span class="sxs-lookup"><span data-stu-id="569f2-117">User Account type, per Windows definition.</span></span> <span data-ttu-id="569f2-118">可能な値は、`unknown`、`standard`、`power`、`administrator` です。</span><span class="sxs-lookup"><span data-stu-id="569f2-118">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="569f2-119">firstSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="569f2-119">firstSeenDateTime</span></span>|<span data-ttu-id="569f2-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="569f2-120">DateTimeOffset</span></span>|<span data-ttu-id="569f2-121">このユーザー アカウントで最初のログオンが発生した日時 (プロバイダーが指定した期間)。</span><span class="sxs-lookup"><span data-stu-id="569f2-121">DateTime at which the earliest logon by this user account occurred (provider-determined period).</span></span> <span data-ttu-id="569f2-122">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="569f2-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="569f2-123">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="569f2-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="569f2-124">lastSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="569f2-124">lastSeenDateTime</span></span>|<span data-ttu-id="569f2-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="569f2-125">DateTimeOffset</span></span>|<span data-ttu-id="569f2-126">このユーザー アカウントで最新のログオンが発生した日時。</span><span class="sxs-lookup"><span data-stu-id="569f2-126">DateTime at which the latest logon by this user account occurred.</span></span> <span data-ttu-id="569f2-127">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="569f2-127">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="569f2-128">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="569f2-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="569f2-129">logonId</span><span class="sxs-lookup"><span data-stu-id="569f2-129">logonId</span></span>|<span data-ttu-id="569f2-130">String</span><span class="sxs-lookup"><span data-stu-id="569f2-130">String</span></span>|<span data-ttu-id="569f2-131">ユーザー ログオン ID</span><span class="sxs-lookup"><span data-stu-id="569f2-131">User logon ID.</span></span>|
|<span data-ttu-id="569f2-132">logonTypes</span><span class="sxs-lookup"><span data-stu-id="569f2-132">logonTypes</span></span>|<span data-ttu-id="569f2-133">String コレクション</span><span class="sxs-lookup"><span data-stu-id="569f2-133">String collection</span></span>|<span data-ttu-id="569f2-134">最初に最後に表示されたときからログオンしたユーザーを確認するログオンの種類のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="569f2-134">Collection of the logon types observed for the logged on user from when first to last seen.</span></span> <span data-ttu-id="569f2-135">使用可能な値: `unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。</span><span class="sxs-lookup"><span data-stu-id="569f2-135">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="569f2-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="569f2-136">JSON representation</span></span>

<span data-ttu-id="569f2-137">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="569f2-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.logonUser"
}-->

```json
{
  "accountDomain": "String",
  "accountName": "String",
  "accountType": "String",
  "firstSeenDateTime": "String (timestamp)",
  "lastSeenDateTime": "String (timestamp)",
  "logonId": "String",
  "logonTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "logonUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->