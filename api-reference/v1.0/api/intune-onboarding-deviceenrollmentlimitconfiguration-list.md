---
title: deviceEnrollmentLimitConfigurations のリスト
description: deviceEnrollmentLimitConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 01f1dff263a5b612b92d403c730f1dbf4e29e317
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974753"
---
# <a name="list-deviceenrollmentlimitconfigurations"></a><span data-ttu-id="79686-103">deviceEnrollmentLimitConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="79686-103">List deviceEnrollmentLimitConfigurations</span></span>

> <span data-ttu-id="79686-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="79686-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79686-105">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="79686-105">List properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79686-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="79686-106">Prerequisites</span></span>
<span data-ttu-id="79686-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79686-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79686-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="79686-109">Permission type</span></span>|<span data-ttu-id="79686-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="79686-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79686-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="79686-111">Delegated (work or school account)</span></span>|<span data-ttu-id="79686-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="79686-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="79686-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="79686-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79686-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79686-114">Not supported.</span></span>|
|<span data-ttu-id="79686-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="79686-115">Application</span></span>|<span data-ttu-id="79686-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79686-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79686-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="79686-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="79686-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79686-118">Request headers</span></span>
|<span data-ttu-id="79686-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79686-119">Header</span></span>|<span data-ttu-id="79686-120">値</span><span class="sxs-lookup"><span data-stu-id="79686-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79686-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="79686-121">Authorization</span></span>|<span data-ttu-id="79686-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="79686-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79686-123">承諾</span><span class="sxs-lookup"><span data-stu-id="79686-123">Accept</span></span>|<span data-ttu-id="79686-124">application/json</span><span class="sxs-lookup"><span data-stu-id="79686-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79686-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="79686-125">Request body</span></span>
<span data-ttu-id="79686-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="79686-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79686-127">応答</span><span class="sxs-lookup"><span data-stu-id="79686-127">Response</span></span>
<span data-ttu-id="79686-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="79686-128">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79686-129">例</span><span class="sxs-lookup"><span data-stu-id="79686-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="79686-130">要求</span><span class="sxs-lookup"><span data-stu-id="79686-130">Request</span></span>
<span data-ttu-id="79686-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="79686-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="79686-132">応答</span><span class="sxs-lookup"><span data-stu-id="79686-132">Response</span></span>
<span data-ttu-id="79686-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="79686-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 446

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
      "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7,
      "limit": 5
    }
  ]
}
```



