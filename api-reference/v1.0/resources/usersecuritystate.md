---
title: userSecurityState リソースの種類
description: ユーザーアカウントに関するステートフルな情報を含みます。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9f5a856a9ec04eaf9a04b82e2ed7697a6735ad88
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033475"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="84945-103">userSecurityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="84945-103">userSecurityState resource type</span></span>

<span data-ttu-id="84945-104">ユーザーアカウントに関するステートフルな情報を含みます。</span><span class="sxs-lookup"><span data-stu-id="84945-104">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="84945-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84945-105">Properties</span></span>

| <span data-ttu-id="84945-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84945-106">Property</span></span>   | <span data-ttu-id="84945-107">型</span><span class="sxs-lookup"><span data-stu-id="84945-107">Type</span></span> |<span data-ttu-id="84945-108">説明</span><span class="sxs-lookup"><span data-stu-id="84945-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84945-109">Usersecuritystate</span><span class="sxs-lookup"><span data-stu-id="84945-109">aadUserId</span></span>|<span data-ttu-id="84945-110">String</span><span class="sxs-lookup"><span data-stu-id="84945-110">String</span></span>|<span data-ttu-id="84945-111">AAD User オブジェクト識別子 (GUID)-物理/マルチアカウントユーザーエンティティを表します。</span><span class="sxs-lookup"><span data-stu-id="84945-111">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="84945-112">accountName</span><span class="sxs-lookup"><span data-stu-id="84945-112">accountName</span></span>|<span data-ttu-id="84945-113">String</span><span class="sxs-lookup"><span data-stu-id="84945-113">String</span></span>|<span data-ttu-id="84945-114">ユーザーアカウントのアカウント名 (Active Directory ドメインまたは DNS ドメインなし)-(と`mailNickName`も呼ばれます)。</span><span class="sxs-lookup"><span data-stu-id="84945-114">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="84945-115">domainName</span><span class="sxs-lookup"><span data-stu-id="84945-115">domainName</span></span>|<span data-ttu-id="84945-116">String</span><span class="sxs-lookup"><span data-stu-id="84945-116">String</span></span>|<span data-ttu-id="84945-117">ユーザーアカウントの NetBIOS/Active Directory ドメイン (つまり、"ドメイン \ ユーザー名" の形式)。</span><span class="sxs-lookup"><span data-stu-id="84945-117">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="84945-118">emailRole</span><span class="sxs-lookup"><span data-stu-id="84945-118">emailRole</span></span>|<span data-ttu-id="84945-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="84945-119">emailRole</span></span>|<span data-ttu-id="84945-120">電子メール関連の警告の場合-ユーザーアカウントの電子メール ' ロール '。</span><span class="sxs-lookup"><span data-stu-id="84945-120">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="84945-121">可能な値は、`unknown`、`sender`、`recipient` です。</span><span class="sxs-lookup"><span data-stu-id="84945-121">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="84945-122">isVpn</span><span class="sxs-lookup"><span data-stu-id="84945-122">isVpn</span></span>|<span data-ttu-id="84945-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="84945-123">Boolean</span></span>|<span data-ttu-id="84945-124">ユーザーが VPN を介してログオンしたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="84945-124">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="84945-125">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="84945-125">logonDateTime</span></span>|<span data-ttu-id="84945-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84945-126">DateTimeOffset</span></span>|<span data-ttu-id="84945-127">サインインが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="84945-127">Time at which the sign-in occurred.</span></span> <span data-ttu-id="84945-128">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="84945-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="84945-129">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="84945-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="84945-130">logonId</span><span class="sxs-lookup"><span data-stu-id="84945-130">logonId</span></span>|<span data-ttu-id="84945-131">String</span><span class="sxs-lookup"><span data-stu-id="84945-131">String</span></span>|<span data-ttu-id="84945-132">ユーザーのサインイン ID。</span><span class="sxs-lookup"><span data-stu-id="84945-132">User sign-in ID.</span></span>|
|<span data-ttu-id="84945-133">logonIp</span><span class="sxs-lookup"><span data-stu-id="84945-133">logonIp</span></span>|<span data-ttu-id="84945-134">String</span><span class="sxs-lookup"><span data-stu-id="84945-134">String</span></span>|<span data-ttu-id="84945-135">サインイン要求の送信元の IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="84945-135">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="84945-136">logonLocation</span><span class="sxs-lookup"><span data-stu-id="84945-136">logonLocation</span></span>|<span data-ttu-id="84945-137">String</span><span class="sxs-lookup"><span data-stu-id="84945-137">String</span></span>|<span data-ttu-id="84945-138">このユーザーによってユーザーのサインインイベントに関連付けられている場所 (IP アドレスマッピング)。</span><span class="sxs-lookup"><span data-stu-id="84945-138">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="84945-139">logonType</span><span class="sxs-lookup"><span data-stu-id="84945-139">logonType</span></span>|<span data-ttu-id="84945-140">logonType</span><span class="sxs-lookup"><span data-stu-id="84945-140">logonType</span></span>|<span data-ttu-id="84945-141">ユーザーのサインイン方法。</span><span class="sxs-lookup"><span data-stu-id="84945-141">Method of user sign in.</span></span> <span data-ttu-id="84945-142">使用可能な値: `unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。</span><span class="sxs-lookup"><span data-stu-id="84945-142">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="84945-143">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="84945-143">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="84945-144">String</span><span class="sxs-lookup"><span data-stu-id="84945-144">String</span></span>|<span data-ttu-id="84945-145">ユーザーの Active Directory (社内) セキュリティ識別子 (SID)。</span><span class="sxs-lookup"><span data-stu-id="84945-145">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="84945-146">riskScore</span><span class="sxs-lookup"><span data-stu-id="84945-146">riskScore</span></span>|<span data-ttu-id="84945-147">String</span><span class="sxs-lookup"><span data-stu-id="84945-147">String</span></span>|<span data-ttu-id="84945-148">ユーザーアカウントのプロバイダーが生成/計算したリスクスコア。</span><span class="sxs-lookup"><span data-stu-id="84945-148">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="84945-149">推奨値の範囲0-1。パーセンテージに相当します。</span><span class="sxs-lookup"><span data-stu-id="84945-149">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="84945-150">userAccountType</span><span class="sxs-lookup"><span data-stu-id="84945-150">userAccountType</span></span>|<span data-ttu-id="84945-151">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="84945-151">userAccountSecurityType</span></span>|<span data-ttu-id="84945-152">ユーザーアカウントの種類 (グループメンバーシップ) (Windows 定義あたり)。</span><span class="sxs-lookup"><span data-stu-id="84945-152">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="84945-153">使用可能な値は、`unknown`、`standard`、`power`、`administrator` です。</span><span class="sxs-lookup"><span data-stu-id="84945-153">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="84945-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="84945-154">userPrincipalName</span></span>|<span data-ttu-id="84945-155">String</span><span class="sxs-lookup"><span data-stu-id="84945-155">String</span></span>|<span data-ttu-id="84945-156">ユーザーのサインイン名-インターネット形式: (ユーザーアカウント名) @ (ユーザーアカウントの DNS ドメイン名)。</span><span class="sxs-lookup"><span data-stu-id="84945-156">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="84945-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="84945-157">JSON representation</span></span>

<span data-ttu-id="84945-158">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="84945-158">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSecurityState"
}-->

```json
{
  "aadUserId": "String",
  "accountName": "String",
  "domainName": "String",
  "emailRole": "@odata.type: microsoft.graph.emailRole",
  "isVpn": true,
  "logonDateTime": "String (timestamp)",
  "logonId": "String",
  "logonIp": "String",
  "logonLocation": "String",
  "logonType": "@odata.type: microsoft.graph.logonType",
  "onPremisesSecurityIdentifier": "String",
  "riskScore": "String",
  "userAccountType": "@odata.type: microsoft.graph.userAccountSecurityType",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
