---
title: managedMobileApps のリスト
description: managedMobileApp オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe3b9e09b51a6b01c6c6af84d4202c81e8b980fd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32529612"
---
# <a name="list-managedmobileapps"></a><span data-ttu-id="bdbb4-103">managedMobileApps のリスト</span><span class="sxs-lookup"><span data-stu-id="bdbb4-103">List managedMobileApps</span></span>

> <span data-ttu-id="bdbb4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bdbb4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bdbb4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bdbb4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdbb4-106">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="bdbb4-106">List properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bdbb4-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="bdbb4-107">Prerequisites</span></span>
<span data-ttu-id="bdbb4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bdbb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdbb4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bdbb4-110">Permission type</span></span>|<span data-ttu-id="bdbb4-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bdbb4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bdbb4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bdbb4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bdbb4-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdbb4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bdbb4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bdbb4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bdbb4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bdbb4-115">Not supported.</span></span>|
|<span data-ttu-id="bdbb4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bdbb4-116">Application</span></span>|<span data-ttu-id="bdbb4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bdbb4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bdbb4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bdbb4-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="bdbb4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bdbb4-119">Request headers</span></span>
|<span data-ttu-id="bdbb4-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bdbb4-120">Header</span></span>|<span data-ttu-id="bdbb4-121">値</span><span class="sxs-lookup"><span data-stu-id="bdbb4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bdbb4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdbb4-122">Authorization</span></span>|<span data-ttu-id="bdbb4-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="bdbb4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bdbb4-124">承諾</span><span class="sxs-lookup"><span data-stu-id="bdbb4-124">Accept</span></span>|<span data-ttu-id="bdbb4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bdbb4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdbb4-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="bdbb4-126">Request body</span></span>
<span data-ttu-id="bdbb4-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bdbb4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bdbb4-128">応答</span><span class="sxs-lookup"><span data-stu-id="bdbb4-128">Response</span></span>
<span data-ttu-id="bdbb4-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedMobileApp](../resources/intune-mam-managedmobileapp.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="bdbb4-129">If successful, this method returns a `200 OK` response code and a collection of [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdbb4-130">例</span><span class="sxs-lookup"><span data-stu-id="bdbb4-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="bdbb4-131">要求</span><span class="sxs-lookup"><span data-stu-id="bdbb4-131">Request</span></span>
<span data-ttu-id="bdbb4-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bdbb4-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
```

### <a name="response"></a><span data-ttu-id="bdbb4-133">応答</span><span class="sxs-lookup"><span data-stu-id="bdbb4-133">Response</span></span>
<span data-ttu-id="bdbb4-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bdbb4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





