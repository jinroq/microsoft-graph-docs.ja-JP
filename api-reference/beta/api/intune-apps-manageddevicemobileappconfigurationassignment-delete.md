---
title: managedDeviceMobileAppConfigurationAssignment の削除
description: managedDeviceMobileAppConfigurationAssignment を削除します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dfb0eb72f1655917168aff2f577313af57739ef1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35961666"
---
# <a name="delete-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="ebcff-103">managedDeviceMobileAppConfigurationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="ebcff-103">Delete managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="ebcff-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebcff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebcff-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ebcff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebcff-106">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="ebcff-106">Deletes a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ebcff-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ebcff-107">Prerequisites</span></span>
<span data-ttu-id="ebcff-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ebcff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebcff-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ebcff-110">Permission type</span></span>|<span data-ttu-id="ebcff-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ebcff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebcff-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ebcff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ebcff-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebcff-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ebcff-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ebcff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebcff-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebcff-115">Not supported.</span></span>|
|<span data-ttu-id="ebcff-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ebcff-116">Application</span></span>|<span data-ttu-id="ebcff-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebcff-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebcff-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ebcff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="ebcff-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ebcff-119">Request headers</span></span>
|<span data-ttu-id="ebcff-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ebcff-120">Header</span></span>|<span data-ttu-id="ebcff-121">値</span><span class="sxs-lookup"><span data-stu-id="ebcff-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebcff-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebcff-122">Authorization</span></span>|<span data-ttu-id="ebcff-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ebcff-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebcff-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ebcff-124">Accept</span></span>|<span data-ttu-id="ebcff-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ebcff-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebcff-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ebcff-126">Request body</span></span>
<span data-ttu-id="ebcff-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ebcff-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebcff-128">応答</span><span class="sxs-lookup"><span data-stu-id="ebcff-128">Response</span></span>
<span data-ttu-id="ebcff-129">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="ebcff-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ebcff-130">例</span><span class="sxs-lookup"><span data-stu-id="ebcff-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebcff-131">要求</span><span class="sxs-lookup"><span data-stu-id="ebcff-131">Request</span></span>
<span data-ttu-id="ebcff-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ebcff-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="ebcff-133">応答</span><span class="sxs-lookup"><span data-stu-id="ebcff-133">Response</span></span>
<span data-ttu-id="ebcff-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ebcff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





