---
title: assign アクション
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: b1f786bec3ce59ac36c12790e09fdcc2cd9a0d78
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319321"
---
# <a name="assign-action"></a><span data-ttu-id="a1b7e-103">assign アクション</span><span class="sxs-lookup"><span data-stu-id="a1b7e-103">assign action</span></span>

> <span data-ttu-id="a1b7e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a1b7e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1b7e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1b7e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a1b7e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a1b7e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1b7e-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a1b7e-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a1b7e-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a1b7e-108">Prerequisites</span></span>
<span data-ttu-id="a1b7e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a1b7e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1b7e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a1b7e-111">Permission type</span></span>|<span data-ttu-id="a1b7e-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a1b7e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1b7e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a1b7e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1b7e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1b7e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a1b7e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a1b7e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1b7e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1b7e-116">Not supported.</span></span>|
|<span data-ttu-id="a1b7e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a1b7e-117">Application</span></span>|<span data-ttu-id="a1b7e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1b7e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1b7e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a1b7e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="a1b7e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a1b7e-120">Request headers</span></span>
|<span data-ttu-id="a1b7e-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a1b7e-121">Header</span></span>|<span data-ttu-id="a1b7e-122">値</span><span class="sxs-lookup"><span data-stu-id="a1b7e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1b7e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1b7e-123">Authorization</span></span>|<span data-ttu-id="a1b7e-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a1b7e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1b7e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a1b7e-125">Accept</span></span>|<span data-ttu-id="a1b7e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a1b7e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1b7e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a1b7e-127">Request body</span></span>
<span data-ttu-id="a1b7e-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a1b7e-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a1b7e-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="a1b7e-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a1b7e-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1b7e-130">Property</span></span>|<span data-ttu-id="a1b7e-131">種類</span><span class="sxs-lookup"><span data-stu-id="a1b7e-131">Type</span></span>|<span data-ttu-id="a1b7e-132">説明</span><span class="sxs-lookup"><span data-stu-id="a1b7e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1b7e-133">appProvisioningConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="a1b7e-133">appProvisioningConfigurationGroupAssignments</span></span>|<span data-ttu-id="a1b7e-134">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a1b7e-134">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) collection</span></span>|<span data-ttu-id="a1b7e-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a1b7e-135">Not yet documented</span></span>|
|<span data-ttu-id="a1b7e-136">iOSLobAppProvisioningConfigAssignments</span><span class="sxs-lookup"><span data-stu-id="a1b7e-136">iOSLobAppProvisioningConfigAssignments</span></span>|<span data-ttu-id="a1b7e-137">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a1b7e-137">[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) collection</span></span>|<span data-ttu-id="a1b7e-138">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a1b7e-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a1b7e-139">応答</span><span class="sxs-lookup"><span data-stu-id="a1b7e-139">Response</span></span>
<span data-ttu-id="a1b7e-140">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="a1b7e-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a1b7e-141">例</span><span class="sxs-lookup"><span data-stu-id="a1b7e-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="a1b7e-142">要求</span><span class="sxs-lookup"><span data-stu-id="a1b7e-142">Request</span></span>
<span data-ttu-id="a1b7e-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a1b7e-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assign

Content-type: application/json
Content-length: 578

{
  "appProvisioningConfigurationGroupAssignments": [
    {
      "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
      "targetGroupId": "Target Group Id value",
      "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
    }
  ],
  "iOSLobAppProvisioningConfigAssignments": [
    {
      "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
      "id": "eac7008e-008e-eac7-8e00-c7ea8e00c7ea",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="a1b7e-144">応答</span><span class="sxs-lookup"><span data-stu-id="a1b7e-144">Response</span></span>
<span data-ttu-id="a1b7e-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a1b7e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




