---
title: windowsDefenderUpdateSignatures アクション
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: e8e613863d33195b5aa99524823048f74227d9c0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316717"
---
# <a name="windowsdefenderupdatesignatures-action"></a><span data-ttu-id="40caa-103">windowsDefenderUpdateSignatures アクション</span><span class="sxs-lookup"><span data-stu-id="40caa-103">windowsDefenderUpdateSignatures action</span></span>

> <span data-ttu-id="40caa-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="40caa-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40caa-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="40caa-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="40caa-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="40caa-106">Prerequisites</span></span>
<span data-ttu-id="40caa-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="40caa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40caa-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="40caa-109">Permission type</span></span>|<span data-ttu-id="40caa-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="40caa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40caa-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="40caa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="40caa-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="40caa-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="40caa-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="40caa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40caa-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40caa-114">Not supported.</span></span>|
|<span data-ttu-id="40caa-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="40caa-115">Application</span></span>|<span data-ttu-id="40caa-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40caa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40caa-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="40caa-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
POST /deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
```

## <a name="request-headers"></a><span data-ttu-id="40caa-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40caa-118">Request headers</span></span>
|<span data-ttu-id="40caa-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40caa-119">Header</span></span>|<span data-ttu-id="40caa-120">値</span><span class="sxs-lookup"><span data-stu-id="40caa-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40caa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="40caa-121">Authorization</span></span>|<span data-ttu-id="40caa-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="40caa-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40caa-123">Accept</span><span class="sxs-lookup"><span data-stu-id="40caa-123">Accept</span></span>|<span data-ttu-id="40caa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="40caa-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40caa-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="40caa-125">Request body</span></span>
<span data-ttu-id="40caa-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="40caa-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40caa-127">応答</span><span class="sxs-lookup"><span data-stu-id="40caa-127">Response</span></span>
<span data-ttu-id="40caa-128">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="40caa-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="40caa-129">例</span><span class="sxs-lookup"><span data-stu-id="40caa-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="40caa-130">要求</span><span class="sxs-lookup"><span data-stu-id="40caa-130">Request</span></span>
<span data-ttu-id="40caa-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="40caa-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
```

### <a name="response"></a><span data-ttu-id="40caa-132">応答</span><span class="sxs-lookup"><span data-stu-id="40caa-132">Response</span></span>
<span data-ttu-id="40caa-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="40caa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



