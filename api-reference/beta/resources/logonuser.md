---
title: logonUser リソースの種類
description: このホストにログオンしているユーザーに関するステートフルな情報を含みます。
localization_priority: Normal
ms.openlocfilehash: 3b7862555c62eb16aaceaa53d4df58541426e08a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562658"
---
# <a name="logonuser-resource-type"></a><span data-ttu-id="263c9-103">logonUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="263c9-103">logonUser resource type</span></span>

<span data-ttu-id="263c9-104">このホストにログオンしているユーザーに関するステートフルな情報を含みます。</span><span class="sxs-lookup"><span data-stu-id="263c9-104">Contains stateful information about the logged on user on this host</span></span>

## <a name="properties"></a><span data-ttu-id="263c9-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="263c9-105">Properties</span></span>

| <span data-ttu-id="263c9-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="263c9-106">Property</span></span>   | <span data-ttu-id="263c9-107">型</span><span class="sxs-lookup"><span data-stu-id="263c9-107">Type</span></span> |<span data-ttu-id="263c9-108">説明</span><span class="sxs-lookup"><span data-stu-id="263c9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="263c9-109">accountdomain</span><span class="sxs-lookup"><span data-stu-id="263c9-109">accountDomain</span></span>|<span data-ttu-id="263c9-110">String</span><span class="sxs-lookup"><span data-stu-id="263c9-110">String</span></span>|<span data-ttu-id="263c9-111">ログオンに使用されるユーザーアカウントのドメイン。</span><span class="sxs-lookup"><span data-stu-id="263c9-111">Domain of user account used to logon.</span></span>|
|<span data-ttu-id="263c9-112">accountName</span><span class="sxs-lookup"><span data-stu-id="263c9-112">accountName</span></span>|<span data-ttu-id="263c9-113">String</span><span class="sxs-lookup"><span data-stu-id="263c9-113">String</span></span>|<span data-ttu-id="263c9-114">ログオンに使用されるユーザーアカウントのアカウント名。</span><span class="sxs-lookup"><span data-stu-id="263c9-114">Account name of user account used to logon.</span></span>|
|<span data-ttu-id="263c9-115">accountType</span><span class="sxs-lookup"><span data-stu-id="263c9-115">accountType</span></span>|<span data-ttu-id="263c9-116">String</span><span class="sxs-lookup"><span data-stu-id="263c9-116">String</span></span>|<span data-ttu-id="263c9-117">ユーザーアカウントの種類 (Windows 定義あたり)。</span><span class="sxs-lookup"><span data-stu-id="263c9-117">User Account type, per Windows definition.</span></span> <span data-ttu-id="263c9-118">使用可能な値は、`unknown`、`standard`、`power`、`administrator` です。</span><span class="sxs-lookup"><span data-stu-id="263c9-118">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="263c9-119">firstseendatetime</span><span class="sxs-lookup"><span data-stu-id="263c9-119">firstSeenDateTime</span></span>|<span data-ttu-id="263c9-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="263c9-120">DateTimeOffset</span></span>|<span data-ttu-id="263c9-121">このユーザーアカウントによる最も早いログオンが発生した日時 (プロバイダーが決定した期間)。</span><span class="sxs-lookup"><span data-stu-id="263c9-121">DateTime at which the earliest logon by this user account occurred (provider-determined period).</span></span> <span data-ttu-id="263c9-122">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="263c9-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="263c9-123">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="263c9-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="263c9-124">lastseendatetime</span><span class="sxs-lookup"><span data-stu-id="263c9-124">lastSeenDateTime</span></span>|<span data-ttu-id="263c9-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="263c9-125">DateTimeOffset</span></span>|<span data-ttu-id="263c9-126">このユーザーアカウントによる最新のログオンが発生した DateTime。</span><span class="sxs-lookup"><span data-stu-id="263c9-126">DateTime at which the latest logon by this user account occurred.</span></span> <span data-ttu-id="263c9-127">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="263c9-127">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="263c9-128">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="263c9-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="263c9-129">logonId</span><span class="sxs-lookup"><span data-stu-id="263c9-129">logonId</span></span>|<span data-ttu-id="263c9-130">String</span><span class="sxs-lookup"><span data-stu-id="263c9-130">String</span></span>|<span data-ttu-id="263c9-131">ユーザーログオン ID。</span><span class="sxs-lookup"><span data-stu-id="263c9-131">User logon ID.</span></span>|
|<span data-ttu-id="263c9-132">logonTypes</span><span class="sxs-lookup"><span data-stu-id="263c9-132">logonTypes</span></span>|<span data-ttu-id="263c9-133">String collection</span><span class="sxs-lookup"><span data-stu-id="263c9-133">String collection</span></span>|<span data-ttu-id="263c9-134">最初に表示された時点から、ログオンしているユーザーに対して観測されたログオンの種類のコレクション。</span><span class="sxs-lookup"><span data-stu-id="263c9-134">Collection of the logon types observed for the logged on user from when first to last seen.</span></span> <span data-ttu-id="263c9-135">使用可能な値: `unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。</span><span class="sxs-lookup"><span data-stu-id="263c9-135">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="263c9-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="263c9-136">JSON representation</span></span>

<span data-ttu-id="263c9-137">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="263c9-137">The following is a JSON representation of the resource.</span></span>

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
