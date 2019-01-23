---
title: リスト windowsInformationProtectionWipeActions
description: WindowsInformationProtectionWipeAction オブジェクトのプロパティと関係を一覧表示します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 07780e126239d808856e5a2e44e63cd75fc3747c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430295"
---
# <a name="list-windowsinformationprotectionwipeactions"></a><span data-ttu-id="9560c-103">リスト windowsInformationProtectionWipeActions</span><span class="sxs-lookup"><span data-stu-id="9560c-103">List windowsInformationProtectionWipeActions</span></span>

> <span data-ttu-id="9560c-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9560c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9560c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9560c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9560c-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9560c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9560c-107">[WindowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="9560c-107">List properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9560c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9560c-108">Prerequisites</span></span>
<span data-ttu-id="9560c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9560c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9560c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9560c-111">Permission type</span></span>|<span data-ttu-id="9560c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9560c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9560c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9560c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9560c-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9560c-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9560c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9560c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9560c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9560c-116">Not supported.</span></span>|
|<span data-ttu-id="9560c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9560c-117">Application</span></span>|<span data-ttu-id="9560c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9560c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9560c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9560c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionWipeActions
```

## <a name="request-headers"></a><span data-ttu-id="9560c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9560c-120">Request headers</span></span>
|<span data-ttu-id="9560c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9560c-121">Header</span></span>|<span data-ttu-id="9560c-122">値</span><span class="sxs-lookup"><span data-stu-id="9560c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9560c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9560c-123">Authorization</span></span>|<span data-ttu-id="9560c-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9560c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9560c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9560c-125">Accept</span></span>|<span data-ttu-id="9560c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9560c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9560c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9560c-127">Request body</span></span>
<span data-ttu-id="9560c-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9560c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9560c-129">応答</span><span class="sxs-lookup"><span data-stu-id="9560c-129">Response</span></span>
<span data-ttu-id="9560c-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="9560c-130">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9560c-131">例</span><span class="sxs-lookup"><span data-stu-id="9560c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9560c-132">要求</span><span class="sxs-lookup"><span data-stu-id="9560c-132">Request</span></span>
<span data-ttu-id="9560c-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9560c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions
```

### <a name="response"></a><span data-ttu-id="9560c-134">応答</span><span class="sxs-lookup"><span data-stu-id="9560c-134">Response</span></span>
<span data-ttu-id="9560c-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9560c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 460

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
      "id": "2620a996-a996-2620-96a9-202696a92026",
      "status": "pending",
      "targetedUserId": "Targeted User Id value",
      "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
      "targetedDeviceName": "Targeted Device Name value",
      "targetedDeviceMacAddress": "Targeted Device Mac Address value"
    }
  ]
}
```




