---
title: revokeUserLicense アクション
description: 指定したアプリに割り当てられた iOS VPP ユーザーライセンスを取り消します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3d1d43181a33cc84ad808af1ce70665b9492922d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35951527"
---
# <a name="revokeuserlicense-action"></a><span data-ttu-id="52d12-103">revokeUserLicense アクション</span><span class="sxs-lookup"><span data-stu-id="52d12-103">revokeUserLicense action</span></span>

> <span data-ttu-id="52d12-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52d12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52d12-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="52d12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52d12-106">指定したアプリに割り当てられた iOS VPP ユーザーライセンスを取り消します。</span><span class="sxs-lookup"><span data-stu-id="52d12-106">Revoke assigned iOS VPP user license for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52d12-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="52d12-107">Prerequisites</span></span>
<span data-ttu-id="52d12-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="52d12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52d12-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="52d12-110">Permission type</span></span>|<span data-ttu-id="52d12-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="52d12-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52d12-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="52d12-112">Delegated (work or school account)</span></span>|<span data-ttu-id="52d12-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52d12-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="52d12-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="52d12-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52d12-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52d12-115">Not supported.</span></span>|
|<span data-ttu-id="52d12-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="52d12-116">Application</span></span>|<span data-ttu-id="52d12-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52d12-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52d12-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="52d12-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeUserLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeUserLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeUserLicense
```

## <a name="request-headers"></a><span data-ttu-id="52d12-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="52d12-119">Request headers</span></span>
|<span data-ttu-id="52d12-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="52d12-120">Header</span></span>|<span data-ttu-id="52d12-121">値</span><span class="sxs-lookup"><span data-stu-id="52d12-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52d12-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="52d12-122">Authorization</span></span>|<span data-ttu-id="52d12-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="52d12-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52d12-124">承諾</span><span class="sxs-lookup"><span data-stu-id="52d12-124">Accept</span></span>|<span data-ttu-id="52d12-125">application/json</span><span class="sxs-lookup"><span data-stu-id="52d12-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52d12-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="52d12-126">Request body</span></span>
<span data-ttu-id="52d12-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="52d12-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="52d12-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="52d12-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="52d12-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52d12-129">Property</span></span>|<span data-ttu-id="52d12-130">型</span><span class="sxs-lookup"><span data-stu-id="52d12-130">Type</span></span>|<span data-ttu-id="52d12-131">説明</span><span class="sxs-lookup"><span data-stu-id="52d12-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52d12-132">userId</span><span class="sxs-lookup"><span data-stu-id="52d12-132">userId</span></span>|<span data-ttu-id="52d12-133">String</span><span class="sxs-lookup"><span data-stu-id="52d12-133">String</span></span>|<span data-ttu-id="52d12-134">割り当てられたアプリライセンスの失効を取り消すユーザー Id</span><span class="sxs-lookup"><span data-stu-id="52d12-134">UserId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="52d12-135">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="52d12-135">notifyManagedDevices</span></span>|<span data-ttu-id="52d12-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="52d12-136">Boolean</span></span>|<span data-ttu-id="52d12-137">失効通知をデバイスに送信する必要があるかどうかを示すブール値</span><span class="sxs-lookup"><span data-stu-id="52d12-137">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="52d12-138">応答</span><span class="sxs-lookup"><span data-stu-id="52d12-138">Response</span></span>
<span data-ttu-id="52d12-139">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="52d12-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="52d12-140">例</span><span class="sxs-lookup"><span data-stu-id="52d12-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="52d12-141">要求</span><span class="sxs-lookup"><span data-stu-id="52d12-141">Request</span></span>
<span data-ttu-id="52d12-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="52d12-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeUserLicense

Content-type: application/json
Content-length: 66

{
  "userId": "User Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="52d12-143">応答</span><span class="sxs-lookup"><span data-stu-id="52d12-143">Response</span></span>
<span data-ttu-id="52d12-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="52d12-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





