---
title: IosEasEmailProfileConfiguration を削除します。
description: IosEasEmailProfileConfiguration を削除します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6daf60e83d136f49946978808b4f2b5c5f5da7de
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837395"
---
# <a name="delete-ioseasemailprofileconfiguration"></a><span data-ttu-id="f5b01-103">IosEasEmailProfileConfiguration を削除します。</span><span class="sxs-lookup"><span data-stu-id="f5b01-103">Delete iosEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="f5b01-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f5b01-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5b01-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5b01-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f5b01-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f5b01-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5b01-107">の[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="f5b01-107">Deletes a [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f5b01-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="f5b01-108">Prerequisites</span></span>
<span data-ttu-id="f5b01-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5b01-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5b01-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f5b01-111">Permission type</span></span>|<span data-ttu-id="f5b01-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f5b01-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5b01-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f5b01-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f5b01-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5b01-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f5b01-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f5b01-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5b01-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5b01-116">Not supported.</span></span>|
|<span data-ttu-id="f5b01-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f5b01-117">Application</span></span>|<span data-ttu-id="f5b01-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5b01-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5b01-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f5b01-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f5b01-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f5b01-120">Request headers</span></span>
|<span data-ttu-id="f5b01-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f5b01-121">Header</span></span>|<span data-ttu-id="f5b01-122">値</span><span class="sxs-lookup"><span data-stu-id="f5b01-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5b01-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5b01-123">Authorization</span></span>|<span data-ttu-id="f5b01-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f5b01-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5b01-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f5b01-125">Accept</span></span>|<span data-ttu-id="f5b01-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f5b01-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5b01-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f5b01-127">Request body</span></span>
<span data-ttu-id="f5b01-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f5b01-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5b01-129">応答</span><span class="sxs-lookup"><span data-stu-id="f5b01-129">Response</span></span>
<span data-ttu-id="f5b01-130">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="f5b01-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f5b01-131">例</span><span class="sxs-lookup"><span data-stu-id="f5b01-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f5b01-132">要求</span><span class="sxs-lookup"><span data-stu-id="f5b01-132">Request</span></span>
<span data-ttu-id="f5b01-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f5b01-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="f5b01-134">応答</span><span class="sxs-lookup"><span data-stu-id="f5b01-134">Response</span></span>
<span data-ttu-id="f5b01-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f5b01-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





