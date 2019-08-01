---
title: logoutSharedAppleDeviceActiveUser アクション
description: 共有の Apple デバイスのアクティブなユーザーをログアウトする
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5f37148835d7e16be3591a844a4a24fe9b7a128d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020991"
---
# <a name="logoutsharedappledeviceactiveuser-action"></a><span data-ttu-id="ee2f6-103">logoutSharedAppleDeviceActiveUser アクション</span><span class="sxs-lookup"><span data-stu-id="ee2f6-103">logoutSharedAppleDeviceActiveUser action</span></span>

> <span data-ttu-id="ee2f6-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ee2f6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee2f6-105">共有の Apple デバイスのアクティブなユーザーをログアウトする</span><span class="sxs-lookup"><span data-stu-id="ee2f6-105">Logout shared Apple device active user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee2f6-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="ee2f6-106">Prerequisites</span></span>
<span data-ttu-id="ee2f6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee2f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee2f6-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ee2f6-109">Permission type</span></span>|<span data-ttu-id="ee2f6-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ee2f6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee2f6-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ee2f6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ee2f6-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="ee2f6-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="ee2f6-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ee2f6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee2f6-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee2f6-114">Not supported.</span></span>|
|<span data-ttu-id="ee2f6-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ee2f6-115">Application</span></span>|<span data-ttu-id="ee2f6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee2f6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee2f6-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ee2f6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/logoutSharedAppleDeviceActiveUser
POST /deviceManagement/managedDevices/{managedDeviceId}/logoutSharedAppleDeviceActiveUser
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/logoutSharedAppleDeviceActiveUser
```

## <a name="request-headers"></a><span data-ttu-id="ee2f6-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee2f6-118">Request headers</span></span>
|<span data-ttu-id="ee2f6-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee2f6-119">Header</span></span>|<span data-ttu-id="ee2f6-120">値</span><span class="sxs-lookup"><span data-stu-id="ee2f6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee2f6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee2f6-121">Authorization</span></span>|<span data-ttu-id="ee2f6-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ee2f6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee2f6-123">承諾</span><span class="sxs-lookup"><span data-stu-id="ee2f6-123">Accept</span></span>|<span data-ttu-id="ee2f6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ee2f6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee2f6-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ee2f6-125">Request body</span></span>
<span data-ttu-id="ee2f6-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ee2f6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee2f6-127">応答</span><span class="sxs-lookup"><span data-stu-id="ee2f6-127">Response</span></span>
<span data-ttu-id="ee2f6-128">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="ee2f6-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ee2f6-129">例</span><span class="sxs-lookup"><span data-stu-id="ee2f6-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee2f6-130">要求</span><span class="sxs-lookup"><span data-stu-id="ee2f6-130">Request</span></span>
<span data-ttu-id="ee2f6-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ee2f6-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/logoutSharedAppleDeviceActiveUser
```

### <a name="response"></a><span data-ttu-id="ee2f6-132">応答</span><span class="sxs-lookup"><span data-stu-id="ee2f6-132">Response</span></span>
<span data-ttu-id="ee2f6-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ee2f6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



