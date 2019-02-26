---
title: detectedApps のリスト
description: detectedApp オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2e96953ec216cb288fcc6660a6a4e7b504b9b149
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256694"
---
# <a name="list-detectedapps"></a><span data-ttu-id="d2998-103">detectedApps のリスト</span><span class="sxs-lookup"><span data-stu-id="d2998-103">List detectedApps</span></span>

> <span data-ttu-id="d2998-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d2998-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2998-105">[detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="d2998-105">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2998-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="d2998-106">Prerequisites</span></span>
<span data-ttu-id="d2998-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2998-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d2998-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d2998-109">Permission type</span></span>|<span data-ttu-id="d2998-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d2998-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2998-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d2998-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d2998-112">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2998-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d2998-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d2998-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2998-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2998-114">Not supported.</span></span>|
|<span data-ttu-id="d2998-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d2998-115">Application</span></span>|<span data-ttu-id="d2998-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2998-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2998-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d2998-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="d2998-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2998-118">Request headers</span></span>
|<span data-ttu-id="d2998-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2998-119">Header</span></span>|<span data-ttu-id="d2998-120">値</span><span class="sxs-lookup"><span data-stu-id="d2998-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2998-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2998-121">Authorization</span></span>|<span data-ttu-id="d2998-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d2998-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2998-123">承諾</span><span class="sxs-lookup"><span data-stu-id="d2998-123">Accept</span></span>|<span data-ttu-id="d2998-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d2998-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2998-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d2998-125">Request body</span></span>
<span data-ttu-id="d2998-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d2998-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2998-127">応答</span><span class="sxs-lookup"><span data-stu-id="d2998-127">Response</span></span>
<span data-ttu-id="d2998-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d2998-128">If successful, this method returns a `200 OK` response code and a collection of [detectedApp](../resources/intune-devices-detectedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2998-129">例</span><span class="sxs-lookup"><span data-stu-id="d2998-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2998-130">要求</span><span class="sxs-lookup"><span data-stu-id="d2998-130">Request</span></span>
<span data-ttu-id="d2998-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d2998-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps
```

### <a name="response"></a><span data-ttu-id="d2998-132">応答</span><span class="sxs-lookup"><span data-stu-id="d2998-132">Response</span></span>
<span data-ttu-id="d2998-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d2998-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.detectedApp",
      "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
      "displayName": "Display Name value",
      "version": "Version value",
      "sizeInByte": 10,
      "deviceCount": 11
    }
  ]
}
```



