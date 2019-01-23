---
title: Delete detectedApp
description: detectedApp を削除します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 91b2515d107ccc4a3b7003360bd76e2f08e7de32
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393110"
---
# <a name="delete-detectedapp"></a><span data-ttu-id="7e0c7-103">Delete detectedApp</span><span class="sxs-lookup"><span data-stu-id="7e0c7-103">Delete detectedApp</span></span>

> <span data-ttu-id="7e0c7-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7e0c7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7e0c7-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e0c7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7e0c7-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7e0c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e0c7-107">[detectedApp](../resources/intune-devices-detectedapp.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="7e0c7-107">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e0c7-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7e0c7-108">Prerequisites</span></span>
<span data-ttu-id="7e0c7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7e0c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7e0c7-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7e0c7-111">Permission type</span></span>|<span data-ttu-id="7e0c7-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7e0c7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e0c7-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7e0c7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7e0c7-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e0c7-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7e0c7-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7e0c7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e0c7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e0c7-116">Not supported.</span></span>|
|<span data-ttu-id="7e0c7-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7e0c7-117">Application</span></span>|<span data-ttu-id="7e0c7-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e0c7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e0c7-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7e0c7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/detectedApps/{detectedAppId}
DELETE /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="7e0c7-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7e0c7-120">Request headers</span></span>
|<span data-ttu-id="7e0c7-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7e0c7-121">Header</span></span>|<span data-ttu-id="7e0c7-122">値</span><span class="sxs-lookup"><span data-stu-id="7e0c7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e0c7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e0c7-123">Authorization</span></span>|<span data-ttu-id="7e0c7-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7e0c7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e0c7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7e0c7-125">Accept</span></span>|<span data-ttu-id="7e0c7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7e0c7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e0c7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7e0c7-127">Request body</span></span>
<span data-ttu-id="7e0c7-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7e0c7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e0c7-129">応答</span><span class="sxs-lookup"><span data-stu-id="7e0c7-129">Response</span></span>
<span data-ttu-id="7e0c7-130">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="7e0c7-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7e0c7-131">例</span><span class="sxs-lookup"><span data-stu-id="7e0c7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e0c7-132">要求</span><span class="sxs-lookup"><span data-stu-id="7e0c7-132">Request</span></span>
<span data-ttu-id="7e0c7-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7e0c7-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/detectedApps/{detectedAppId}
```

### <a name="response"></a><span data-ttu-id="7e0c7-134">応答</span><span class="sxs-lookup"><span data-stu-id="7e0c7-134">Response</span></span>
<span data-ttu-id="7e0c7-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7e0c7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




