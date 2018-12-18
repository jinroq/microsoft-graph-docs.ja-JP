---
title: logoutSharedAppleDeviceActiveUser アクション
description: 共有の Apple デバイスのアクティブなユーザーをログアウトする
author: tfitzmac
ms.openlocfilehash: 7f88f050e38d7d352b43722a7e0a71fca2fa4fb6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302066"
---
# <a name="logoutsharedappledeviceactiveuser-action"></a><span data-ttu-id="83975-103">logoutSharedAppleDeviceActiveUser アクション</span><span class="sxs-lookup"><span data-stu-id="83975-103">logoutSharedAppleDeviceActiveUser action</span></span>

> <span data-ttu-id="83975-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="83975-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83975-105">共有の Apple デバイスのアクティブなユーザーをログアウトする</span><span class="sxs-lookup"><span data-stu-id="83975-105">Logout shared Apple device active user</span></span>
## <a name="prerequisites"></a><span data-ttu-id="83975-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="83975-106">Prerequisites</span></span>
<span data-ttu-id="83975-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="83975-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83975-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="83975-109">Permission type</span></span>|<span data-ttu-id="83975-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="83975-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83975-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="83975-111">Delegated (work or school account)</span></span>|<span data-ttu-id="83975-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="83975-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="83975-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="83975-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83975-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83975-114">Not supported.</span></span>|
|<span data-ttu-id="83975-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="83975-115">Application</span></span>|<span data-ttu-id="83975-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83975-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83975-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="83975-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/logoutSharedAppleDeviceActiveUser
POST /deviceManagement/managedDevices/{managedDeviceId}/logoutSharedAppleDeviceActiveUser
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/logoutSharedAppleDeviceActiveUser
```

## <a name="request-headers"></a><span data-ttu-id="83975-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="83975-118">Request headers</span></span>
|<span data-ttu-id="83975-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="83975-119">Header</span></span>|<span data-ttu-id="83975-120">値</span><span class="sxs-lookup"><span data-stu-id="83975-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83975-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="83975-121">Authorization</span></span>|<span data-ttu-id="83975-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="83975-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83975-123">Accept</span><span class="sxs-lookup"><span data-stu-id="83975-123">Accept</span></span>|<span data-ttu-id="83975-124">application/json</span><span class="sxs-lookup"><span data-stu-id="83975-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83975-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="83975-125">Request body</span></span>
<span data-ttu-id="83975-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="83975-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83975-127">応答</span><span class="sxs-lookup"><span data-stu-id="83975-127">Response</span></span>
<span data-ttu-id="83975-128">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="83975-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="83975-129">例</span><span class="sxs-lookup"><span data-stu-id="83975-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="83975-130">要求</span><span class="sxs-lookup"><span data-stu-id="83975-130">Request</span></span>
<span data-ttu-id="83975-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="83975-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/logoutSharedAppleDeviceActiveUser
```

### <a name="response"></a><span data-ttu-id="83975-132">応答</span><span class="sxs-lookup"><span data-stu-id="83975-132">Response</span></span>
<span data-ttu-id="83975-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="83975-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



