---
title: userSecurityState リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 62a54a996d7fe9c892da797cee352a57d0782035
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517240"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="d7cac-104">userSecurityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d7cac-104">userSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7cac-105">ユーザー アカウントに関するステートフルな情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d7cac-105">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="d7cac-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7cac-106">Properties</span></span>

| <span data-ttu-id="d7cac-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7cac-107">Property</span></span>   | <span data-ttu-id="d7cac-108">型</span><span class="sxs-lookup"><span data-stu-id="d7cac-108">Type</span></span> |<span data-ttu-id="d7cac-109">説明</span><span class="sxs-lookup"><span data-stu-id="d7cac-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7cac-110">aadUserId</span><span class="sxs-lookup"><span data-stu-id="d7cac-110">aadUserId</span></span>|<span data-ttu-id="d7cac-111">String</span><span class="sxs-lookup"><span data-stu-id="d7cac-111">String</span></span>|<span data-ttu-id="d7cac-112">AAD のユーザーは、物理/マルチ account ユーザー エンティティを表すオブジェクト識別子 (GUID) をします。</span><span class="sxs-lookup"><span data-stu-id="d7cac-112">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="d7cac-113">accountName</span><span class="sxs-lookup"><span data-stu-id="d7cac-113">accountName</span></span>|<span data-ttu-id="d7cac-114">String</span><span class="sxs-lookup"><span data-stu-id="d7cac-114">String</span></span>|<span data-ttu-id="d7cac-115">(せずに Active Directory ドメインまたは DNS ドメイン) のユーザー アカウントのアカウント名 (とも呼ばれる`mailNickName`)。</span><span class="sxs-lookup"><span data-stu-id="d7cac-115">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="d7cac-116">domainName</span><span class="sxs-lookup"><span data-stu-id="d7cac-116">domainName</span></span>|<span data-ttu-id="d7cac-117">String</span><span class="sxs-lookup"><span data-stu-id="d7cac-117">String</span></span>|<span data-ttu-id="d7cac-118">ユーザー アカウント (ドメイン \ アカウントの形式は、) の NetBIOS と Active Directory ドメイン。</span><span class="sxs-lookup"><span data-stu-id="d7cac-118">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="d7cac-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="d7cac-119">emailRole</span></span>|<span data-ttu-id="d7cac-120">emailRole</span><span class="sxs-lookup"><span data-stu-id="d7cac-120">emailRole</span></span>|<span data-ttu-id="d7cac-121">電子メール関連のアラートをユーザー アカウントの電子メール 'ロール'。</span><span class="sxs-lookup"><span data-stu-id="d7cac-121">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="d7cac-122">可能な値は、`unknown`、`sender`、`recipient` です。</span><span class="sxs-lookup"><span data-stu-id="d7cac-122">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="d7cac-123">isVpn</span><span class="sxs-lookup"><span data-stu-id="d7cac-123">isVpn</span></span>|<span data-ttu-id="d7cac-124">ブール値</span><span class="sxs-lookup"><span data-stu-id="d7cac-124">Boolean</span></span>|<span data-ttu-id="d7cac-125">VPN 経由でユーザーをログオンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d7cac-125">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="d7cac-126">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="d7cac-126">logonDateTime</span></span>|<span data-ttu-id="d7cac-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7cac-127">DateTimeOffset</span></span>|<span data-ttu-id="d7cac-128">サインインが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="d7cac-128">Time at which the sign-in occurred.</span></span> <span data-ttu-id="d7cac-129">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="d7cac-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d7cac-130">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。</span><span class="sxs-lookup"><span data-stu-id="d7cac-130">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="d7cac-131">logonId</span><span class="sxs-lookup"><span data-stu-id="d7cac-131">logonId</span></span>|<span data-ttu-id="d7cac-132">String</span><span class="sxs-lookup"><span data-stu-id="d7cac-132">String</span></span>|<span data-ttu-id="d7cac-133">ユーザーのサインイン ID</span><span class="sxs-lookup"><span data-stu-id="d7cac-133">User sign-in ID.</span></span>|
|<span data-ttu-id="d7cac-134">logonIp</span><span class="sxs-lookup"><span data-stu-id="d7cac-134">logonIp</span></span>|<span data-ttu-id="d7cac-135">String</span><span class="sxs-lookup"><span data-stu-id="d7cac-135">String</span></span>|<span data-ttu-id="d7cac-136">IP アドレスは、サインイン要求が出されたからです。</span><span class="sxs-lookup"><span data-stu-id="d7cac-136">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="d7cac-137">logonLocation</span><span class="sxs-lookup"><span data-stu-id="d7cac-137">logonLocation</span></span>|<span data-ttu-id="d7cac-138">String</span><span class="sxs-lookup"><span data-stu-id="d7cac-138">String</span></span>|<span data-ttu-id="d7cac-139">(IP アドレスのマッピング) によって場所がこのユーザー、ユーザーのサインインがイベントに関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="d7cac-139">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="d7cac-140">logonType</span><span class="sxs-lookup"><span data-stu-id="d7cac-140">logonType</span></span>|<span data-ttu-id="d7cac-141">logonType</span><span class="sxs-lookup"><span data-stu-id="d7cac-141">logonType</span></span>|<span data-ttu-id="d7cac-142">ユーザーのサインインの方法です。</span><span class="sxs-lookup"><span data-stu-id="d7cac-142">Method of user sign in.</span></span> <span data-ttu-id="d7cac-143">使用可能な値: `unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。</span><span class="sxs-lookup"><span data-stu-id="d7cac-143">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="d7cac-144">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="d7cac-144">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="d7cac-145">String</span><span class="sxs-lookup"><span data-stu-id="d7cac-145">String</span></span>|<span data-ttu-id="d7cac-146">アクティブなディレクトリ (設置型) のセキュリティ識別子 (SID) ユーザーの。</span><span class="sxs-lookup"><span data-stu-id="d7cac-146">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="d7cac-147">riskScore</span><span class="sxs-lookup"><span data-stu-id="d7cac-147">riskScore</span></span>|<span data-ttu-id="d7cac-148">String</span><span class="sxs-lookup"><span data-stu-id="d7cac-148">String</span></span>|<span data-ttu-id="d7cac-149">ユーザー アカウントのプロバイダーによって生成されると計算されるリスク ・ スコアです。</span><span class="sxs-lookup"><span data-stu-id="d7cac-149">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="d7cac-150">0 - 1 パーセントに相当する値の範囲をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="d7cac-150">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="d7cac-151">userAccountType</span><span class="sxs-lookup"><span data-stu-id="d7cac-151">userAccountType</span></span>|<span data-ttu-id="d7cac-152">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="d7cac-152">userAccountSecurityType</span></span>|<span data-ttu-id="d7cac-153">ユーザー アカウントの種類 (グループ) は、Windows の定義ごと。</span><span class="sxs-lookup"><span data-stu-id="d7cac-153">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="d7cac-154">可能な値は、`unknown`、`standard`、`power`、`administrator` です。</span><span class="sxs-lookup"><span data-stu-id="d7cac-154">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="d7cac-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d7cac-155">userPrincipalName</span></span>|<span data-ttu-id="d7cac-156">文字列</span><span class="sxs-lookup"><span data-stu-id="d7cac-156">String</span></span>|<span data-ttu-id="d7cac-157">ユーザー サインイン名をインターネット形式: (ユーザー アカウント名) @(ユーザー アカウントの DNS ドメイン名) です。</span><span class="sxs-lookup"><span data-stu-id="d7cac-157">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d7cac-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d7cac-158">JSON representation</span></span>

<span data-ttu-id="d7cac-159">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d7cac-159">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "userSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/usersecuritystate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
