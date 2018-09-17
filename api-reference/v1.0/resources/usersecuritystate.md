# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="c9674-101">userSecurityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c9674-101">userSecurityState resource type</span></span>

<span data-ttu-id="c9674-102">ユーザー アカウントに関するステートフルな情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c9674-102">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="c9674-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9674-103">Properties</span></span>

| <span data-ttu-id="c9674-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9674-104">Property</span></span>   | <span data-ttu-id="c9674-105">型</span><span class="sxs-lookup"><span data-stu-id="c9674-105">Type</span></span> |<span data-ttu-id="c9674-106">説明</span><span class="sxs-lookup"><span data-stu-id="c9674-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9674-107">aadUserId</span><span class="sxs-lookup"><span data-stu-id="c9674-107">aadUserId</span></span>|<span data-ttu-id="c9674-108">文字列</span><span class="sxs-lookup"><span data-stu-id="c9674-108">String</span></span>|<span data-ttu-id="c9674-109">AAD のユーザーは、物理/マルチ account ユーザー エンティティを表すオブジェクト識別子 (GUID) をします。</span><span class="sxs-lookup"><span data-stu-id="c9674-109">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="c9674-110">accountName</span><span class="sxs-lookup"><span data-stu-id="c9674-110">accountName</span></span>|<span data-ttu-id="c9674-111">文字列</span><span class="sxs-lookup"><span data-stu-id="c9674-111">String</span></span>|<span data-ttu-id="c9674-112">(せずに Active Directory ドメインまたは DNS ドメイン) のユーザー アカウントのアカウント名 (とも呼ばれる `mailNickName`)。</span><span class="sxs-lookup"><span data-stu-id="c9674-112">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="c9674-113">domainName</span><span class="sxs-lookup"><span data-stu-id="c9674-113">domainName</span></span>|<span data-ttu-id="c9674-114">文字列</span><span class="sxs-lookup"><span data-stu-id="c9674-114">String</span></span>|<span data-ttu-id="c9674-115">ユーザー アカウント (ドメイン \ アカウントの形式は、) の NetBIOS と Active Directory ドメイン。</span><span class="sxs-lookup"><span data-stu-id="c9674-115">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="c9674-116">emailRole</span><span class="sxs-lookup"><span data-stu-id="c9674-116">emailRole</span></span>|<span data-ttu-id="c9674-117">emailRole</span><span class="sxs-lookup"><span data-stu-id="c9674-117">emailRole</span></span>|<span data-ttu-id="c9674-118">電子メール関連のアラートをユーザー アカウントの電子メール 'ロール'。</span><span class="sxs-lookup"><span data-stu-id="c9674-118">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="c9674-119">可能な値は、`unknown`、`sender`、`recipient` です。</span><span class="sxs-lookup"><span data-stu-id="c9674-119">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="c9674-120">isVpn</span><span class="sxs-lookup"><span data-stu-id="c9674-120">isVpn</span></span>|<span data-ttu-id="c9674-121">ブール値</span><span class="sxs-lookup"><span data-stu-id="c9674-121">Boolean</span></span>|<span data-ttu-id="c9674-122">VPN 経由でユーザーをログオンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c9674-122">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="c9674-123">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="c9674-123">logonDateTime</span></span>|<span data-ttu-id="c9674-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9674-124">DateTimeOffset</span></span>|<span data-ttu-id="c9674-125">サインインが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="c9674-125">Time at which the sign-in occurred.</span></span> <span data-ttu-id="c9674-126">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="c9674-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c9674-127">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります `'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="c9674-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="c9674-128">logonId</span><span class="sxs-lookup"><span data-stu-id="c9674-128">logonId</span></span>|<span data-ttu-id="c9674-129">文字列</span><span class="sxs-lookup"><span data-stu-id="c9674-129">String</span></span>|<span data-ttu-id="c9674-130">ユーザーのサインイン ID</span><span class="sxs-lookup"><span data-stu-id="c9674-130">User sign-in ID.</span></span>|
|<span data-ttu-id="c9674-131">logonIp</span><span class="sxs-lookup"><span data-stu-id="c9674-131">logonIp</span></span>|<span data-ttu-id="c9674-132">文字列</span><span class="sxs-lookup"><span data-stu-id="c9674-132">String</span></span>|<span data-ttu-id="c9674-133">IP アドレスは、サインイン要求が出されたからです。</span><span class="sxs-lookup"><span data-stu-id="c9674-133">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="c9674-134">logonLocation</span><span class="sxs-lookup"><span data-stu-id="c9674-134">logonLocation</span></span>|<span data-ttu-id="c9674-135">文字列</span><span class="sxs-lookup"><span data-stu-id="c9674-135">String</span></span>|<span data-ttu-id="c9674-136">(IP アドレスのマッピング) によって場所がこのユーザー、ユーザーのサインインがイベントに関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="c9674-136">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="c9674-137">logonType</span><span class="sxs-lookup"><span data-stu-id="c9674-137">logonType</span></span>|<span data-ttu-id="c9674-138">logonType</span><span class="sxs-lookup"><span data-stu-id="c9674-138">logonType</span></span>|<span data-ttu-id="c9674-139">ユーザーのサインイン方法。</span><span class="sxs-lookup"><span data-stu-id="c9674-139">Method of user sign in.</span></span> <span data-ttu-id="c9674-140">可能な値は、`unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service` です。</span><span class="sxs-lookup"><span data-stu-id="c9674-140">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="c9674-141">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="c9674-141">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="c9674-142">文字列</span><span class="sxs-lookup"><span data-stu-id="c9674-142">String</span></span>|<span data-ttu-id="c9674-143">アクティブなディレクトリ (設置型) のセキュリティ識別子 (SID) ユーザーの。</span><span class="sxs-lookup"><span data-stu-id="c9674-143">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="c9674-144">riskScore</span><span class="sxs-lookup"><span data-stu-id="c9674-144">riskScore</span></span>|<span data-ttu-id="c9674-145">文字列</span><span class="sxs-lookup"><span data-stu-id="c9674-145">String</span></span>|<span data-ttu-id="c9674-146">ユーザー アカウントのプロバイダーによって生成されると計算されるリスク ・ スコアです。</span><span class="sxs-lookup"><span data-stu-id="c9674-146">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="c9674-147">パーセンテージに相当する 0 - 1 の値の範囲を推奨します。</span><span class="sxs-lookup"><span data-stu-id="c9674-147">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="c9674-148">userAccountType</span><span class="sxs-lookup"><span data-stu-id="c9674-148">userAccountType</span></span>|<span data-ttu-id="c9674-149">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="c9674-149">userAccountSecurityType</span></span>|<span data-ttu-id="c9674-150">ユーザー アカウントの種類 (グループ) は、Windows の定義ごと。</span><span class="sxs-lookup"><span data-stu-id="c9674-150">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="c9674-151">可能な値は、`unknown`、`standard`、`power`、`administrator` です。</span><span class="sxs-lookup"><span data-stu-id="c9674-151">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="c9674-152">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c9674-152">userPrincipalName</span></span>|<span data-ttu-id="c9674-153">文字列</span><span class="sxs-lookup"><span data-stu-id="c9674-153">String</span></span>|<span data-ttu-id="c9674-154">ユーザー サインイン名をインターネット形式: (ユーザー アカウント名) @(ユーザー アカウントの DNS ドメイン名) です。</span><span class="sxs-lookup"><span data-stu-id="c9674-154">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9674-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c9674-155">JSON representation</span></span>

<span data-ttu-id="c9674-156">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c9674-156">The following is a JSON representation of the resource.</span></span>

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
