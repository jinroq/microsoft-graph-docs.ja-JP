---
title: managedMobileApps のリスト
description: managedMobileApp オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fa2983cc8b6088acfa739b3be3dd1f904bfab739
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35996617"
---
# <a name="list-managedmobileapps"></a><span data-ttu-id="6b6d2-103">managedMobileApps のリスト</span><span class="sxs-lookup"><span data-stu-id="6b6d2-103">List managedMobileApps</span></span>

> <span data-ttu-id="6b6d2-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6b6d2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b6d2-105">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6b6d2-105">List properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b6d2-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="6b6d2-106">Prerequisites</span></span>
<span data-ttu-id="6b6d2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b6d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b6d2-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6b6d2-109">Permission type</span></span>|<span data-ttu-id="6b6d2-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6b6d2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b6d2-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6b6d2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6b6d2-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b6d2-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6b6d2-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6b6d2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b6d2-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b6d2-114">Not supported.</span></span>|
|<span data-ttu-id="6b6d2-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6b6d2-115">Application</span></span>|<span data-ttu-id="6b6d2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b6d2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b6d2-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6b6d2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps
```

## <a name="request-headers"></a><span data-ttu-id="6b6d2-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6b6d2-118">Request headers</span></span>
|<span data-ttu-id="6b6d2-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6b6d2-119">Header</span></span>|<span data-ttu-id="6b6d2-120">値</span><span class="sxs-lookup"><span data-stu-id="6b6d2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b6d2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b6d2-121">Authorization</span></span>|<span data-ttu-id="6b6d2-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6b6d2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b6d2-123">承諾</span><span class="sxs-lookup"><span data-stu-id="6b6d2-123">Accept</span></span>|<span data-ttu-id="6b6d2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6b6d2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b6d2-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="6b6d2-125">Request body</span></span>
<span data-ttu-id="6b6d2-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6b6d2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b6d2-127">応答</span><span class="sxs-lookup"><span data-stu-id="6b6d2-127">Response</span></span>
<span data-ttu-id="6b6d2-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="6b6d2-128">If successful, this method returns a `200 OK` response code and a collection of [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b6d2-129">例</span><span class="sxs-lookup"><span data-stu-id="6b6d2-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b6d2-130">要求</span><span class="sxs-lookup"><span data-stu-id="6b6d2-130">Request</span></span>
<span data-ttu-id="6b6d2-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6b6d2-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
```

### <a name="response"></a><span data-ttu-id="6b6d2-132">応答</span><span class="sxs-lookup"><span data-stu-id="6b6d2-132">Response</span></span>
<span data-ttu-id="6b6d2-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6b6d2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```



