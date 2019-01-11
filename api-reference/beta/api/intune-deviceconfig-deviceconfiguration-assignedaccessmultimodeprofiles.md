---
title: assignedAccessMultiModeProfiles アクション
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 09183d5328b7dbbc92fa6052990e71b40df838ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828078"
---
# <a name="assignedaccessmultimodeprofiles-action"></a><span data-ttu-id="92951-103">assignedAccessMultiModeProfiles アクション</span><span class="sxs-lookup"><span data-stu-id="92951-103">assignedAccessMultiModeProfiles action</span></span>

> <span data-ttu-id="92951-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="92951-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92951-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92951-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="92951-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="92951-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="92951-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="92951-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="92951-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="92951-108">Prerequisites</span></span>
<span data-ttu-id="92951-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="92951-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92951-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="92951-111">Permission type</span></span>|<span data-ttu-id="92951-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="92951-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92951-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="92951-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92951-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="92951-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="92951-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="92951-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92951-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92951-116">Not supported.</span></span>|
|<span data-ttu-id="92951-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="92951-117">Application</span></span>|<span data-ttu-id="92951-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92951-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92951-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="92951-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
```

## <a name="request-headers"></a><span data-ttu-id="92951-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="92951-120">Request headers</span></span>
|<span data-ttu-id="92951-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="92951-121">Header</span></span>|<span data-ttu-id="92951-122">値</span><span class="sxs-lookup"><span data-stu-id="92951-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92951-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="92951-123">Authorization</span></span>|<span data-ttu-id="92951-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="92951-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92951-125">Accept</span><span class="sxs-lookup"><span data-stu-id="92951-125">Accept</span></span>|<span data-ttu-id="92951-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92951-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92951-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="92951-127">Request body</span></span>
<span data-ttu-id="92951-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="92951-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="92951-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="92951-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="92951-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92951-130">Property</span></span>|<span data-ttu-id="92951-131">種類</span><span class="sxs-lookup"><span data-stu-id="92951-131">Type</span></span>|<span data-ttu-id="92951-132">説明</span><span class="sxs-lookup"><span data-stu-id="92951-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92951-133">assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="92951-133">assignedAccessMultiModeProfiles</span></span>|<span data-ttu-id="92951-134">[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="92951-134">[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) collection</span></span>|<span data-ttu-id="92951-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="92951-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="92951-136">応答</span><span class="sxs-lookup"><span data-stu-id="92951-136">Response</span></span>
<span data-ttu-id="92951-137">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="92951-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="92951-138">例</span><span class="sxs-lookup"><span data-stu-id="92951-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="92951-139">要求</span><span class="sxs-lookup"><span data-stu-id="92951-139">Request</span></span>
<span data-ttu-id="92951-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="92951-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="92951-141">応答</span><span class="sxs-lookup"><span data-stu-id="92951-141">Response</span></span>
<span data-ttu-id="92951-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="92951-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





