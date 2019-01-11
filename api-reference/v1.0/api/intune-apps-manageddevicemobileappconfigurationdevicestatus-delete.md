---
title: ManagedDeviceMobileAppConfigurationDeviceStatus を削除します。
description: ManagedDeviceMobileAppConfigurationDeviceStatus を削除します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9053b3f86b8809f4920b7d10c157e40fe58ba4f9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867320"
---
# <a name="delete-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="961aa-103">ManagedDeviceMobileAppConfigurationDeviceStatus を削除します。</span><span class="sxs-lookup"><span data-stu-id="961aa-103">Delete managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="961aa-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="961aa-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="961aa-105">の[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="961aa-105">Deletes a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="961aa-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="961aa-106">Prerequisites</span></span>
<span data-ttu-id="961aa-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="961aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="961aa-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="961aa-109">Permission type</span></span>|<span data-ttu-id="961aa-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="961aa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="961aa-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="961aa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="961aa-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="961aa-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="961aa-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="961aa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="961aa-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="961aa-114">Not supported.</span></span>|
|<span data-ttu-id="961aa-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="961aa-115">Application</span></span>|<span data-ttu-id="961aa-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="961aa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="961aa-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="961aa-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="961aa-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="961aa-118">Request headers</span></span>
|<span data-ttu-id="961aa-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="961aa-119">Header</span></span>|<span data-ttu-id="961aa-120">値</span><span class="sxs-lookup"><span data-stu-id="961aa-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="961aa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="961aa-121">Authorization</span></span>|<span data-ttu-id="961aa-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="961aa-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="961aa-123">Accept</span><span class="sxs-lookup"><span data-stu-id="961aa-123">Accept</span></span>|<span data-ttu-id="961aa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="961aa-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="961aa-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="961aa-125">Request body</span></span>
<span data-ttu-id="961aa-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="961aa-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="961aa-127">応答</span><span class="sxs-lookup"><span data-stu-id="961aa-127">Response</span></span>
<span data-ttu-id="961aa-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="961aa-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="961aa-129">例</span><span class="sxs-lookup"><span data-stu-id="961aa-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="961aa-130">要求</span><span class="sxs-lookup"><span data-stu-id="961aa-130">Request</span></span>
<span data-ttu-id="961aa-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="961aa-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="961aa-132">応答</span><span class="sxs-lookup"><span data-stu-id="961aa-132">Response</span></span>
<span data-ttu-id="961aa-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="961aa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



