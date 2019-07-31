---
title: リスト mobileAppTroubleshootingEvents
description: 複数のワークフローをサポートする Microsoft Graph API for Intune の List mobileAppTroubleshootingEvent メソッドについて説明します。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7e3f25d4116d2dcbb577be968bf880e785d498b5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993565"
---
# <a name="list-mobileapptroubleshootingevents"></a><span data-ttu-id="a0ea8-103">リスト mobileAppTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="a0ea8-103">List mobileAppTroubleshootingEvents</span></span>

> <span data-ttu-id="a0ea8-104">**重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="a0ea8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a0ea8-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a0ea8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a0ea8-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a0ea8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0ea8-107">[MobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a0ea8-107">List properties and relationships of the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0ea8-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a0ea8-108">Prerequisites</span></span>
<span data-ttu-id="a0ea8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a0ea8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0ea8-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a0ea8-111">Permission type</span></span>|<span data-ttu-id="a0ea8-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a0ea8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0ea8-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a0ea8-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="a0ea8-114">&nbsp;&nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="a0ea8-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="a0ea8-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0ea8-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a0ea8-116">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="a0ea8-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="a0ea8-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0ea8-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a0ea8-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a0ea8-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0ea8-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a0ea8-119">Not supported.</span></span>|
|<span data-ttu-id="a0ea8-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a0ea8-120">Application</span></span>|<span data-ttu-id="a0ea8-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a0ea8-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0ea8-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a0ea8-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents
GET /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="a0ea8-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a0ea8-123">Request headers</span></span>
|<span data-ttu-id="a0ea8-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a0ea8-124">Header</span></span>|<span data-ttu-id="a0ea8-125">値</span><span class="sxs-lookup"><span data-stu-id="a0ea8-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0ea8-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0ea8-126">Authorization</span></span>|<span data-ttu-id="a0ea8-127">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a0ea8-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0ea8-128">承諾</span><span class="sxs-lookup"><span data-stu-id="a0ea8-128">Accept</span></span>|<span data-ttu-id="a0ea8-129">application/json</span><span class="sxs-lookup"><span data-stu-id="a0ea8-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0ea8-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="a0ea8-130">Request body</span></span>
<span data-ttu-id="a0ea8-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a0ea8-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0ea8-132">応答</span><span class="sxs-lookup"><span data-stu-id="a0ea8-132">Response</span></span>
<span data-ttu-id="a0ea8-133">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a0ea8-133">If successful, this method returns a `200 OK` response code and a collection of [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0ea8-134">例</span><span class="sxs-lookup"><span data-stu-id="a0ea8-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0ea8-135">要求</span><span class="sxs-lookup"><span data-stu-id="a0ea8-135">Request</span></span>
<span data-ttu-id="a0ea8-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a0ea8-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="a0ea8-137">応答</span><span class="sxs-lookup"><span data-stu-id="a0ea8-137">Response</span></span>
<span data-ttu-id="a0ea8-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a0ea8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 161

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
      "id": "77943c10-3c10-7794-103c-9477103c9477"
    }
  ]
}
```




