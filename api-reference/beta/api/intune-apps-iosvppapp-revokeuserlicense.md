---
title: revokeUserLicense アクション
description: Revoke が割り当てられている iOS VPP ユーザー ライセンスは、アプリケーションを指定します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5f94cf25824d6e81c609c634c03f5e607fa75dfb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417848"
---
# <a name="revokeuserlicense-action"></a><span data-ttu-id="a9a9e-103">revokeUserLicense アクション</span><span class="sxs-lookup"><span data-stu-id="a9a9e-103">revokeUserLicense action</span></span>

> <span data-ttu-id="a9a9e-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a9a9e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a9a9e-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9a9e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a9a9e-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a9a9e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9a9e-107">Revoke が割り当てられている iOS VPP ユーザー ライセンスは、アプリケーションを指定します。</span><span class="sxs-lookup"><span data-stu-id="a9a9e-107">Revoke assigned iOS VPP user license for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9a9e-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a9a9e-108">Prerequisites</span></span>
<span data-ttu-id="a9a9e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9a9e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a9a9e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a9a9e-111">Permission type</span></span>|<span data-ttu-id="a9a9e-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a9a9e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9a9e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a9a9e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9a9e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9a9e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a9a9e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a9a9e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9a9e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9a9e-116">Not supported.</span></span>|
|<span data-ttu-id="a9a9e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a9a9e-117">Application</span></span>|<span data-ttu-id="a9a9e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9a9e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9a9e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a9a9e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeUserLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeUserLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeUserLicense
```

## <a name="request-headers"></a><span data-ttu-id="a9a9e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a9a9e-120">Request headers</span></span>
|<span data-ttu-id="a9a9e-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a9a9e-121">Header</span></span>|<span data-ttu-id="a9a9e-122">値</span><span class="sxs-lookup"><span data-stu-id="a9a9e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9a9e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9a9e-123">Authorization</span></span>|<span data-ttu-id="a9a9e-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a9a9e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9a9e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a9a9e-125">Accept</span></span>|<span data-ttu-id="a9a9e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9a9e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9a9e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a9a9e-127">Request body</span></span>
<span data-ttu-id="a9a9e-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a9a9e-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a9a9e-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="a9a9e-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a9a9e-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9a9e-130">Property</span></span>|<span data-ttu-id="a9a9e-131">型</span><span class="sxs-lookup"><span data-stu-id="a9a9e-131">Type</span></span>|<span data-ttu-id="a9a9e-132">説明</span><span class="sxs-lookup"><span data-stu-id="a9a9e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9a9e-133">userId</span><span class="sxs-lookup"><span data-stu-id="a9a9e-133">userId</span></span>|<span data-ttu-id="a9a9e-134">String</span><span class="sxs-lookup"><span data-stu-id="a9a9e-134">String</span></span>|<span data-ttu-id="a9a9e-135">ユーザー Id が割り当てられているアプリケーションのライセンスを失効させるのには相手</span><span class="sxs-lookup"><span data-stu-id="a9a9e-135">UserId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="a9a9e-136">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="a9a9e-136">notifyManagedDevices</span></span>|<span data-ttu-id="a9a9e-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9a9e-137">Boolean</span></span>|<span data-ttu-id="a9a9e-138">取り消しの通知をデバイスに送信するかどうかであることを示すブール値</span><span class="sxs-lookup"><span data-stu-id="a9a9e-138">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="a9a9e-139">応答</span><span class="sxs-lookup"><span data-stu-id="a9a9e-139">Response</span></span>
<span data-ttu-id="a9a9e-140">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="a9a9e-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a9a9e-141">例</span><span class="sxs-lookup"><span data-stu-id="a9a9e-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9a9e-142">要求</span><span class="sxs-lookup"><span data-stu-id="a9a9e-142">Request</span></span>
<span data-ttu-id="a9a9e-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a9a9e-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeUserLicense

Content-type: application/json
Content-length: 66

{
  "userId": "User Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="a9a9e-144">応答</span><span class="sxs-lookup"><span data-stu-id="a9a9e-144">Response</span></span>
<span data-ttu-id="a9a9e-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a9a9e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




