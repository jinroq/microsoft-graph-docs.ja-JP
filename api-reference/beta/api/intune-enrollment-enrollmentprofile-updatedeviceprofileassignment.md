---
title: updateDeviceProfileAssignment アクション
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ca2cca2777a2043248257b26da10a6b191c6038e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423315"
---
# <a name="updatedeviceprofileassignment-action"></a><span data-ttu-id="1da7d-103">updateDeviceProfileAssignment アクション</span><span class="sxs-lookup"><span data-stu-id="1da7d-103">updateDeviceProfileAssignment action</span></span>

> <span data-ttu-id="1da7d-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1da7d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1da7d-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1da7d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1da7d-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1da7d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1da7d-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1da7d-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1da7d-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="1da7d-108">Prerequisites</span></span>
<span data-ttu-id="1da7d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1da7d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1da7d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1da7d-111">Permission type</span></span>|<span data-ttu-id="1da7d-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1da7d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1da7d-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1da7d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1da7d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1da7d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1da7d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1da7d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1da7d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1da7d-116">Not supported.</span></span>|
|<span data-ttu-id="1da7d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1da7d-117">Application</span></span>|<span data-ttu-id="1da7d-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1da7d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1da7d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1da7d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/updateDeviceProfileAssignment
```

## <a name="request-headers"></a><span data-ttu-id="1da7d-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1da7d-120">Request headers</span></span>
|<span data-ttu-id="1da7d-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1da7d-121">Header</span></span>|<span data-ttu-id="1da7d-122">値</span><span class="sxs-lookup"><span data-stu-id="1da7d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1da7d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1da7d-123">Authorization</span></span>|<span data-ttu-id="1da7d-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1da7d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1da7d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1da7d-125">Accept</span></span>|<span data-ttu-id="1da7d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1da7d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1da7d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1da7d-127">Request body</span></span>
<span data-ttu-id="1da7d-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1da7d-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1da7d-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="1da7d-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1da7d-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1da7d-130">Property</span></span>|<span data-ttu-id="1da7d-131">型</span><span class="sxs-lookup"><span data-stu-id="1da7d-131">Type</span></span>|<span data-ttu-id="1da7d-132">説明</span><span class="sxs-lookup"><span data-stu-id="1da7d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1da7d-133">deviceIds</span><span class="sxs-lookup"><span data-stu-id="1da7d-133">deviceIds</span></span>|<span data-ttu-id="1da7d-134">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1da7d-134">String collection</span></span>|<span data-ttu-id="1da7d-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1da7d-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1da7d-136">応答</span><span class="sxs-lookup"><span data-stu-id="1da7d-136">Response</span></span>
<span data-ttu-id="1da7d-137">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="1da7d-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1da7d-138">例</span><span class="sxs-lookup"><span data-stu-id="1da7d-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="1da7d-139">要求</span><span class="sxs-lookup"><span data-stu-id="1da7d-139">Request</span></span>
<span data-ttu-id="1da7d-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1da7d-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/updateDeviceProfileAssignment

Content-type: application/json
Content-length: 51

{
  "deviceIds": [
    "Device Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="1da7d-141">応答</span><span class="sxs-lookup"><span data-stu-id="1da7d-141">Response</span></span>
<span data-ttu-id="1da7d-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1da7d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




