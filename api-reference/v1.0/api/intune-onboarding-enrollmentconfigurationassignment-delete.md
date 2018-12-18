---
title: enrollmentConfigurationAssignment の削除
description: enrollmentConfigurationAssignment を削除します。
author: tfitzmac
ms.openlocfilehash: aa809a2a69ec5e40470b9b95e9ca51dec13b9f10
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355035"
---
# <a name="delete-enrollmentconfigurationassignment"></a><span data-ttu-id="74fee-103">enrollmentConfigurationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="74fee-103">Delete enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="74fee-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="74fee-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74fee-105">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="74fee-105">Deletes a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="74fee-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="74fee-106">Prerequisites</span></span>
<span data-ttu-id="74fee-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74fee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74fee-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="74fee-109">Permission type</span></span>|<span data-ttu-id="74fee-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="74fee-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74fee-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="74fee-111">Delegated (work or school account)</span></span>|<span data-ttu-id="74fee-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74fee-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="74fee-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="74fee-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74fee-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74fee-114">Not supported.</span></span>|
|<span data-ttu-id="74fee-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="74fee-115">Application</span></span>|<span data-ttu-id="74fee-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74fee-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74fee-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="74fee-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="74fee-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74fee-118">Request headers</span></span>
|<span data-ttu-id="74fee-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74fee-119">Header</span></span>|<span data-ttu-id="74fee-120">値</span><span class="sxs-lookup"><span data-stu-id="74fee-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74fee-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="74fee-121">Authorization</span></span>|<span data-ttu-id="74fee-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="74fee-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74fee-123">Accept</span><span class="sxs-lookup"><span data-stu-id="74fee-123">Accept</span></span>|<span data-ttu-id="74fee-124">application/json</span><span class="sxs-lookup"><span data-stu-id="74fee-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74fee-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="74fee-125">Request body</span></span>
<span data-ttu-id="74fee-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="74fee-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74fee-127">応答</span><span class="sxs-lookup"><span data-stu-id="74fee-127">Response</span></span>
<span data-ttu-id="74fee-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="74fee-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="74fee-129">例</span><span class="sxs-lookup"><span data-stu-id="74fee-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="74fee-130">要求</span><span class="sxs-lookup"><span data-stu-id="74fee-130">Request</span></span>
<span data-ttu-id="74fee-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="74fee-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="74fee-132">応答</span><span class="sxs-lookup"><span data-stu-id="74fee-132">Response</span></span>
<span data-ttu-id="74fee-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="74fee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



