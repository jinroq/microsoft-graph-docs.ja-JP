---
title: extendQualityUpdatesPause アクション
description: ビジネス リングの Windows の更新プログラムの品質の更新プログラムの一時停止を拡張します。
author: tfitzmac
ms.openlocfilehash: ea6f36922b438e5f643e073c4d5d2697a6f77efc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355609"
---
# <a name="extendqualityupdatespause-action"></a><span data-ttu-id="406c9-103">extendQualityUpdatesPause アクション</span><span class="sxs-lookup"><span data-stu-id="406c9-103">extendQualityUpdatesPause action</span></span>

> <span data-ttu-id="406c9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="406c9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="406c9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="406c9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="406c9-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="406c9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="406c9-107">ビジネス リングの Windows の更新プログラムの品質の更新プログラムの一時停止を拡張します。</span><span class="sxs-lookup"><span data-stu-id="406c9-107">Extend Quality Updates Pause for a Windows Update for Business ring.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="406c9-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="406c9-108">Prerequisites</span></span>
<span data-ttu-id="406c9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="406c9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="406c9-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="406c9-111">Permission type</span></span>|<span data-ttu-id="406c9-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="406c9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="406c9-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="406c9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="406c9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="406c9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="406c9-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="406c9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="406c9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="406c9-116">Not supported.</span></span>|
|<span data-ttu-id="406c9-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="406c9-117">Application</span></span>|<span data-ttu-id="406c9-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="406c9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="406c9-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="406c9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/extendQualityUpdatesPause
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/extendQualityUpdatesPause
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/extendQualityUpdatesPause
```

## <a name="request-headers"></a><span data-ttu-id="406c9-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="406c9-120">Request headers</span></span>
|<span data-ttu-id="406c9-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="406c9-121">Header</span></span>|<span data-ttu-id="406c9-122">値</span><span class="sxs-lookup"><span data-stu-id="406c9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="406c9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="406c9-123">Authorization</span></span>|<span data-ttu-id="406c9-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="406c9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="406c9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="406c9-125">Accept</span></span>|<span data-ttu-id="406c9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="406c9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="406c9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="406c9-127">Request body</span></span>
<span data-ttu-id="406c9-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="406c9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="406c9-129">応答</span><span class="sxs-lookup"><span data-stu-id="406c9-129">Response</span></span>
<span data-ttu-id="406c9-130">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="406c9-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="406c9-131">例</span><span class="sxs-lookup"><span data-stu-id="406c9-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="406c9-132">要求</span><span class="sxs-lookup"><span data-stu-id="406c9-132">Request</span></span>
<span data-ttu-id="406c9-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="406c9-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/extendQualityUpdatesPause
```

### <a name="response"></a><span data-ttu-id="406c9-134">応答</span><span class="sxs-lookup"><span data-stu-id="406c9-134">Response</span></span>
<span data-ttu-id="406c9-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="406c9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





