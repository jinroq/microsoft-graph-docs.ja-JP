---
title: autopilotDeviceStream 関数
description: 自動操縦装置ストリームを使用して、アップロード要求を作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1c03ca0319e3e6458c3a58ea82efb52b6c6bc840
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532451"
---
# <a name="autopilotdevicestream-function"></a><span data-ttu-id="94f1a-103">autopilotDeviceStream 関数</span><span class="sxs-lookup"><span data-stu-id="94f1a-103">autopilotDeviceStream function</span></span>

> <span data-ttu-id="94f1a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94f1a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94f1a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="94f1a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94f1a-106">自動操縦装置ストリームを使用して、アップロード要求を作成します。</span><span class="sxs-lookup"><span data-stu-id="94f1a-106">Create a upload request with autopilot device stream in it.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94f1a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="94f1a-107">Prerequisites</span></span>
<span data-ttu-id="94f1a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="94f1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94f1a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="94f1a-110">Permission type</span></span>|<span data-ttu-id="94f1a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="94f1a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94f1a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="94f1a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="94f1a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94f1a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="94f1a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="94f1a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94f1a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94f1a-115">Not supported.</span></span>|
|<span data-ttu-id="94f1a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="94f1a-116">Application</span></span>|<span data-ttu-id="94f1a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94f1a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94f1a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="94f1a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/autopilotDeviceStream
```

## <a name="request-headers"></a><span data-ttu-id="94f1a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="94f1a-119">Request headers</span></span>
|<span data-ttu-id="94f1a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="94f1a-120">Header</span></span>|<span data-ttu-id="94f1a-121">値</span><span class="sxs-lookup"><span data-stu-id="94f1a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94f1a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="94f1a-122">Authorization</span></span>|<span data-ttu-id="94f1a-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="94f1a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94f1a-124">承諾</span><span class="sxs-lookup"><span data-stu-id="94f1a-124">Accept</span></span>|<span data-ttu-id="94f1a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="94f1a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94f1a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="94f1a-126">Request body</span></span>
<span data-ttu-id="94f1a-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="94f1a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94f1a-128">応答</span><span class="sxs-lookup"><span data-stu-id="94f1a-128">Response</span></span>
<span data-ttu-id="94f1a-129">成功した場合、この関数`200 OK`は応答コードと、応答本文で文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="94f1a-129">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94f1a-130">例</span><span class="sxs-lookup"><span data-stu-id="94f1a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="94f1a-131">要求</span><span class="sxs-lookup"><span data-stu-id="94f1a-131">Request</span></span>
<span data-ttu-id="94f1a-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="94f1a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/autopilotDeviceStream
```

### <a name="response"></a><span data-ttu-id="94f1a-133">応答</span><span class="sxs-lookup"><span data-stu-id="94f1a-133">Response</span></span>
<span data-ttu-id="94f1a-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="94f1a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 48

{
  "value": "Autopilot Device Stream value"
}
```





