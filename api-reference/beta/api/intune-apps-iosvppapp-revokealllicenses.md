---
title: revokeAllLicenses アクション
description: 指定したアプリに割り当てられたすべての iOS VPP ライセンスを取り消します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 65829fa75efefa23d30e2e9628c4c1066eef4e91
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30966517"
---
# <a name="revokealllicenses-action"></a><span data-ttu-id="c03a1-103">revokeAllLicenses アクション</span><span class="sxs-lookup"><span data-stu-id="c03a1-103">revokeAllLicenses action</span></span>

> <span data-ttu-id="c03a1-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c03a1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c03a1-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c03a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c03a1-106">指定したアプリに割り当てられたすべての iOS VPP ライセンスを取り消します。</span><span class="sxs-lookup"><span data-stu-id="c03a1-106">Revoke all assigned iOS VPP licenses for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c03a1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c03a1-107">Prerequisites</span></span>
<span data-ttu-id="c03a1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c03a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c03a1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c03a1-110">Permission type</span></span>|<span data-ttu-id="c03a1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c03a1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c03a1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c03a1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c03a1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c03a1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c03a1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c03a1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c03a1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c03a1-115">Not supported.</span></span>|
|<span data-ttu-id="c03a1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c03a1-116">Application</span></span>|<span data-ttu-id="c03a1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c03a1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c03a1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c03a1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeAllLicenses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeAllLicenses
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeAllLicenses
```

## <a name="request-headers"></a><span data-ttu-id="c03a1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c03a1-119">Request headers</span></span>
|<span data-ttu-id="c03a1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c03a1-120">Header</span></span>|<span data-ttu-id="c03a1-121">値</span><span class="sxs-lookup"><span data-stu-id="c03a1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c03a1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c03a1-122">Authorization</span></span>|<span data-ttu-id="c03a1-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c03a1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c03a1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c03a1-124">Accept</span></span>|<span data-ttu-id="c03a1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c03a1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c03a1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c03a1-126">Request body</span></span>
<span data-ttu-id="c03a1-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c03a1-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c03a1-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="c03a1-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c03a1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c03a1-129">Property</span></span>|<span data-ttu-id="c03a1-130">型</span><span class="sxs-lookup"><span data-stu-id="c03a1-130">Type</span></span>|<span data-ttu-id="c03a1-131">説明</span><span class="sxs-lookup"><span data-stu-id="c03a1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c03a1-132">notifymanageddevices</span><span class="sxs-lookup"><span data-stu-id="c03a1-132">notifyManagedDevices</span></span>|<span data-ttu-id="c03a1-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="c03a1-133">Boolean</span></span>|<span data-ttu-id="c03a1-134">失効通知をデバイスに送信する必要があるかどうかを示すブール値</span><span class="sxs-lookup"><span data-stu-id="c03a1-134">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="c03a1-135">応答</span><span class="sxs-lookup"><span data-stu-id="c03a1-135">Response</span></span>
<span data-ttu-id="c03a1-136">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="c03a1-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c03a1-137">例</span><span class="sxs-lookup"><span data-stu-id="c03a1-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="c03a1-138">要求</span><span class="sxs-lookup"><span data-stu-id="c03a1-138">Request</span></span>
<span data-ttu-id="c03a1-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c03a1-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeAllLicenses

Content-type: application/json
Content-length: 36

{
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="c03a1-140">応答</span><span class="sxs-lookup"><span data-stu-id="c03a1-140">Response</span></span>
<span data-ttu-id="c03a1-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c03a1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




