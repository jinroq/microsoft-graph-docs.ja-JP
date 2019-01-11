---
title: deviceComplianceUserStatus の削除
description: deviceComplianceUserStatus を削除します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6fa4542b28fb49be9d23c0cbfcabdd5ba058c018
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835680"
---
# <a name="delete-devicecomplianceuserstatus"></a><span data-ttu-id="61491-103">deviceComplianceUserStatus の削除</span><span class="sxs-lookup"><span data-stu-id="61491-103">Delete deviceComplianceUserStatus</span></span>

> <span data-ttu-id="61491-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="61491-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61491-105">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="61491-105">Deletes a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="61491-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="61491-106">Prerequisites</span></span>
<span data-ttu-id="61491-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="61491-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61491-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="61491-109">Permission type</span></span>|<span data-ttu-id="61491-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="61491-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61491-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="61491-111">Delegated (work or school account)</span></span>|<span data-ttu-id="61491-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61491-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="61491-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="61491-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61491-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61491-114">Not supported.</span></span>|
|<span data-ttu-id="61491-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="61491-115">Application</span></span>|<span data-ttu-id="61491-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61491-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61491-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="61491-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="61491-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="61491-118">Request headers</span></span>
|<span data-ttu-id="61491-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="61491-119">Header</span></span>|<span data-ttu-id="61491-120">値</span><span class="sxs-lookup"><span data-stu-id="61491-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61491-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="61491-121">Authorization</span></span>|<span data-ttu-id="61491-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="61491-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61491-123">Accept</span><span class="sxs-lookup"><span data-stu-id="61491-123">Accept</span></span>|<span data-ttu-id="61491-124">application/json</span><span class="sxs-lookup"><span data-stu-id="61491-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61491-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="61491-125">Request body</span></span>
<span data-ttu-id="61491-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="61491-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61491-127">応答</span><span class="sxs-lookup"><span data-stu-id="61491-127">Response</span></span>
<span data-ttu-id="61491-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="61491-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="61491-129">例</span><span class="sxs-lookup"><span data-stu-id="61491-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="61491-130">要求</span><span class="sxs-lookup"><span data-stu-id="61491-130">Request</span></span>
<span data-ttu-id="61491-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="61491-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

### <a name="response"></a><span data-ttu-id="61491-132">応答</span><span class="sxs-lookup"><span data-stu-id="61491-132">Response</span></span>
<span data-ttu-id="61491-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="61491-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



