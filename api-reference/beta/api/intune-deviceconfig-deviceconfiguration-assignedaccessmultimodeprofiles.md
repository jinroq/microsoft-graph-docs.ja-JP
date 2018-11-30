---
title: assignedAccessMultiModeProfiles アクション
description: まだ文書化されていません
ms.openlocfilehash: eb4e4cce71baabfcd10d28b88438dd2e4fe989c7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070129"
---
# <a name="assignedaccessmultimodeprofiles-action"></a><span data-ttu-id="86d8b-103">assignedAccessMultiModeProfiles アクション</span><span class="sxs-lookup"><span data-stu-id="86d8b-103">assignedAccessMultiModeProfiles action</span></span>

> <span data-ttu-id="86d8b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="86d8b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="86d8b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86d8b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="86d8b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="86d8b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="86d8b-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="86d8b-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="86d8b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="86d8b-108">Prerequisites</span></span>
<span data-ttu-id="86d8b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="86d8b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86d8b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="86d8b-111">Permission type</span></span>|<span data-ttu-id="86d8b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="86d8b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86d8b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="86d8b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="86d8b-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="86d8b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="86d8b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="86d8b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86d8b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86d8b-116">Not supported.</span></span>|
|<span data-ttu-id="86d8b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="86d8b-117">Application</span></span>|<span data-ttu-id="86d8b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86d8b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86d8b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="86d8b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
```

## <a name="request-headers"></a><span data-ttu-id="86d8b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="86d8b-120">Request headers</span></span>
|<span data-ttu-id="86d8b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="86d8b-121">Header</span></span>|<span data-ttu-id="86d8b-122">値</span><span class="sxs-lookup"><span data-stu-id="86d8b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86d8b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="86d8b-123">Authorization</span></span>|<span data-ttu-id="86d8b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="86d8b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86d8b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="86d8b-125">Accept</span></span>|<span data-ttu-id="86d8b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86d8b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86d8b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="86d8b-127">Request body</span></span>
<span data-ttu-id="86d8b-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="86d8b-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="86d8b-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="86d8b-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="86d8b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86d8b-130">Property</span></span>|<span data-ttu-id="86d8b-131">型</span><span class="sxs-lookup"><span data-stu-id="86d8b-131">Type</span></span>|<span data-ttu-id="86d8b-132">説明</span><span class="sxs-lookup"><span data-stu-id="86d8b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86d8b-133">assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="86d8b-133">assignedAccessMultiModeProfiles</span></span>|<span data-ttu-id="86d8b-134">[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="86d8b-134">[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) collection</span></span>|<span data-ttu-id="86d8b-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="86d8b-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="86d8b-136">応答</span><span class="sxs-lookup"><span data-stu-id="86d8b-136">Response</span></span>
<span data-ttu-id="86d8b-137">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="86d8b-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="86d8b-138">例</span><span class="sxs-lookup"><span data-stu-id="86d8b-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="86d8b-139">要求</span><span class="sxs-lookup"><span data-stu-id="86d8b-139">Request</span></span>
<span data-ttu-id="86d8b-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="86d8b-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles

Content-type: application/json
Content-length: 528

{
  "assignedAccessMultiModeProfiles": [
    {
      "@odata.type": "#microsoft.graph.windowsAssignedAccessProfile",
      "id": "cfa70299-0299-cfa7-9902-a7cf9902a7cf",
      "profileName": "Profile Name value",
      "showTaskBar": true,
      "appUserModelIds": [
        "App User Model Ids value"
      ],
      "desktopAppPaths": [
        "Desktop App Paths value"
      ],
      "userAccounts": [
        "User Accounts value"
      ],
      "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="86d8b-141">応答</span><span class="sxs-lookup"><span data-stu-id="86d8b-141">Response</span></span>
<span data-ttu-id="86d8b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="86d8b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





