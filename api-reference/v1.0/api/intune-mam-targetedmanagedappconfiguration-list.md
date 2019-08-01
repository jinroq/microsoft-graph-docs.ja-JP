---
title: targetedManagedAppConfigurations のリスト
description: targetedManagedAppConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4e501983ef8ff489f36910198e842258231d39a7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020536"
---
# <a name="list-targetedmanagedappconfigurations"></a><span data-ttu-id="260ae-103">targetedManagedAppConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="260ae-103">List targetedManagedAppConfigurations</span></span>

> <span data-ttu-id="260ae-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="260ae-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="260ae-105">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="260ae-105">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="260ae-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="260ae-106">Prerequisites</span></span>
<span data-ttu-id="260ae-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="260ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="260ae-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="260ae-109">Permission type</span></span>|<span data-ttu-id="260ae-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="260ae-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="260ae-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="260ae-111">Delegated (work or school account)</span></span>|<span data-ttu-id="260ae-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="260ae-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="260ae-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="260ae-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="260ae-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="260ae-114">Not supported.</span></span>|
|<span data-ttu-id="260ae-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="260ae-115">Application</span></span>|<span data-ttu-id="260ae-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="260ae-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="260ae-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="260ae-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="260ae-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="260ae-118">Request headers</span></span>
|<span data-ttu-id="260ae-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="260ae-119">Header</span></span>|<span data-ttu-id="260ae-120">値</span><span class="sxs-lookup"><span data-stu-id="260ae-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="260ae-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="260ae-121">Authorization</span></span>|<span data-ttu-id="260ae-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="260ae-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="260ae-123">承諾</span><span class="sxs-lookup"><span data-stu-id="260ae-123">Accept</span></span>|<span data-ttu-id="260ae-124">application/json</span><span class="sxs-lookup"><span data-stu-id="260ae-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="260ae-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="260ae-125">Request body</span></span>
<span data-ttu-id="260ae-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="260ae-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="260ae-127">応答</span><span class="sxs-lookup"><span data-stu-id="260ae-127">Response</span></span>
<span data-ttu-id="260ae-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="260ae-128">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="260ae-129">例</span><span class="sxs-lookup"><span data-stu-id="260ae-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="260ae-130">要求</span><span class="sxs-lookup"><span data-stu-id="260ae-130">Request</span></span>
<span data-ttu-id="260ae-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="260ae-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations
```

### <a name="response"></a><span data-ttu-id="260ae-132">応答</span><span class="sxs-lookup"><span data-stu-id="260ae-132">Response</span></span>
<span data-ttu-id="260ae-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="260ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 657

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "2444e029-e029-2444-29e0-442429e04424",
      "version": "Version value",
      "customSettings": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "deployedAppCount": 0,
      "isAssigned": true
    }
  ]
}
```



