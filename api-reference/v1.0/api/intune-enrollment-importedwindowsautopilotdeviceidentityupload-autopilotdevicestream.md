---
title: autopilotDeviceStream 関数
description: 自動操縦装置ストリームを使用して、アップロード要求を作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9730986d9282abb95f08fb2a297f0b2bb0a3dc6e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578744"
---
# <a name="autopilotdevicestream-function"></a><span data-ttu-id="85771-103">autopilotDeviceStream 関数</span><span class="sxs-lookup"><span data-stu-id="85771-103">autopilotDeviceStream function</span></span>

> <span data-ttu-id="85771-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="85771-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85771-105">自動操縦装置ストリームを使用して、アップロード要求を作成します。</span><span class="sxs-lookup"><span data-stu-id="85771-105">Create a upload request with autopilot device stream in it.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85771-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="85771-106">Prerequisites</span></span>
<span data-ttu-id="85771-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="85771-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85771-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="85771-109">Permission type</span></span>|<span data-ttu-id="85771-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="85771-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85771-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="85771-111">Delegated (work or school account)</span></span>|<span data-ttu-id="85771-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85771-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="85771-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="85771-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85771-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85771-114">Not supported.</span></span>|
|<span data-ttu-id="85771-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="85771-115">Application</span></span>|<span data-ttu-id="85771-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85771-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85771-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="85771-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/autopilotDeviceStream
```

## <a name="request-headers"></a><span data-ttu-id="85771-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="85771-118">Request headers</span></span>
|<span data-ttu-id="85771-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="85771-119">Header</span></span>|<span data-ttu-id="85771-120">値</span><span class="sxs-lookup"><span data-stu-id="85771-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85771-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="85771-121">Authorization</span></span>|<span data-ttu-id="85771-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="85771-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85771-123">承諾</span><span class="sxs-lookup"><span data-stu-id="85771-123">Accept</span></span>|<span data-ttu-id="85771-124">application/json</span><span class="sxs-lookup"><span data-stu-id="85771-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85771-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="85771-125">Request body</span></span>
<span data-ttu-id="85771-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="85771-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85771-127">応答</span><span class="sxs-lookup"><span data-stu-id="85771-127">Response</span></span>
<span data-ttu-id="85771-128">成功した場合、この関数`200 OK`は応答コードと、応答本文で文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="85771-128">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85771-129">例</span><span class="sxs-lookup"><span data-stu-id="85771-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="85771-130">要求</span><span class="sxs-lookup"><span data-stu-id="85771-130">Request</span></span>
<span data-ttu-id="85771-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="85771-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/autopilotDeviceStream
```

### <a name="response"></a><span data-ttu-id="85771-132">応答</span><span class="sxs-lookup"><span data-stu-id="85771-132">Response</span></span>
<span data-ttu-id="85771-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="85771-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 48

{
  "value": "Autopilot Device Stream value"
}
```



