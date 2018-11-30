---
title: WindowsDomainJoinConfiguration を削除します。
description: WindowsDomainJoinConfiguration を削除します。
ms.openlocfilehash: 79126f49689ce9a25b6a0efe8e99e2427225403f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073681"
---
# <a name="delete-windowsdomainjoinconfiguration"></a><span data-ttu-id="6fdff-103">WindowsDomainJoinConfiguration を削除します。</span><span class="sxs-lookup"><span data-stu-id="6fdff-103">Delete windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="6fdff-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6fdff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6fdff-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6fdff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6fdff-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6fdff-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6fdff-107">の[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="6fdff-107">Deletes a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6fdff-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="6fdff-108">Prerequisites</span></span>
<span data-ttu-id="6fdff-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6fdff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fdff-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6fdff-111">Permission type</span></span>|<span data-ttu-id="6fdff-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6fdff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fdff-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6fdff-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6fdff-114">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="6fdff-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="6fdff-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fdff-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="6fdff-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6fdff-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fdff-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6fdff-117">Not supported.</span></span>|
|<span data-ttu-id="6fdff-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6fdff-118">Application</span></span>|<span data-ttu-id="6fdff-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6fdff-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fdff-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6fdff-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6fdff-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6fdff-121">Request headers</span></span>
|<span data-ttu-id="6fdff-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6fdff-122">Header</span></span>|<span data-ttu-id="6fdff-123">値</span><span class="sxs-lookup"><span data-stu-id="6fdff-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fdff-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fdff-124">Authorization</span></span>|<span data-ttu-id="6fdff-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6fdff-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fdff-126">Accept</span><span class="sxs-lookup"><span data-stu-id="6fdff-126">Accept</span></span>|<span data-ttu-id="6fdff-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6fdff-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fdff-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="6fdff-128">Request body</span></span>
<span data-ttu-id="6fdff-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6fdff-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fdff-130">応答</span><span class="sxs-lookup"><span data-stu-id="6fdff-130">Response</span></span>
<span data-ttu-id="6fdff-131">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="6fdff-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6fdff-132">例</span><span class="sxs-lookup"><span data-stu-id="6fdff-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="6fdff-133">要求</span><span class="sxs-lookup"><span data-stu-id="6fdff-133">Request</span></span>
<span data-ttu-id="6fdff-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6fdff-134">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="6fdff-135">応答</span><span class="sxs-lookup"><span data-stu-id="6fdff-135">Response</span></span>
<span data-ttu-id="6fdff-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6fdff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



