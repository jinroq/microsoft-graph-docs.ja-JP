---
title: autopilotDeviceStream 関数
description: 自動操縦装置ストリームを使用して、アップロード要求を作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: df3cd9c7deff70d7cc81f3016d1d08e62c277608
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253716"
---
# <a name="autopilotdevicestream-function"></a><span data-ttu-id="64973-103">autopilotDeviceStream 関数</span><span class="sxs-lookup"><span data-stu-id="64973-103">autopilotDeviceStream function</span></span>

> <span data-ttu-id="64973-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="64973-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64973-105">自動操縦装置ストリームを使用して、アップロード要求を作成します。</span><span class="sxs-lookup"><span data-stu-id="64973-105">Create a upload request with autopilot device stream in it.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64973-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="64973-106">Prerequisites</span></span>
<span data-ttu-id="64973-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="64973-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="64973-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="64973-109">Permission type</span></span>|<span data-ttu-id="64973-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="64973-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64973-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="64973-111">Delegated (work or school account)</span></span>|<span data-ttu-id="64973-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64973-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="64973-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="64973-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64973-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64973-114">Not supported.</span></span>|
|<span data-ttu-id="64973-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="64973-115">Application</span></span>|<span data-ttu-id="64973-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64973-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64973-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="64973-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/autopilotDeviceStream
```

## <a name="request-headers"></a><span data-ttu-id="64973-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="64973-118">Request headers</span></span>
|<span data-ttu-id="64973-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="64973-119">Header</span></span>|<span data-ttu-id="64973-120">値</span><span class="sxs-lookup"><span data-stu-id="64973-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64973-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="64973-121">Authorization</span></span>|<span data-ttu-id="64973-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="64973-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64973-123">承諾</span><span class="sxs-lookup"><span data-stu-id="64973-123">Accept</span></span>|<span data-ttu-id="64973-124">application/json</span><span class="sxs-lookup"><span data-stu-id="64973-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64973-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="64973-125">Request body</span></span>
<span data-ttu-id="64973-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="64973-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64973-127">応答</span><span class="sxs-lookup"><span data-stu-id="64973-127">Response</span></span>
<span data-ttu-id="64973-128">成功した場合、この関数は `200 OK` 応答コードと、応答本文で String を返します。</span><span class="sxs-lookup"><span data-stu-id="64973-128">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64973-129">例</span><span class="sxs-lookup"><span data-stu-id="64973-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="64973-130">要求</span><span class="sxs-lookup"><span data-stu-id="64973-130">Request</span></span>
<span data-ttu-id="64973-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="64973-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/autopilotDeviceStream
```

### <a name="response"></a><span data-ttu-id="64973-132">応答</span><span class="sxs-lookup"><span data-stu-id="64973-132">Response</span></span>
<span data-ttu-id="64973-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="64973-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 48

{
  "value": "Autopilot Device Stream value"
}
```



