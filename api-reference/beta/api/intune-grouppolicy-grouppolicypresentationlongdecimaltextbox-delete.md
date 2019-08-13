---
title: GroupPolicyPresentationLongDecimalTextBox の削除
description: GroupPolicyPresentationLongDecimalTextBox を削除します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5b041d4aa302c08296e7e5c5bf57d322fe10324d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357769"
---
# <a name="delete-grouppolicypresentationlongdecimaltextbox"></a><span data-ttu-id="939dc-103">GroupPolicyPresentationLongDecimalTextBox の削除</span><span class="sxs-lookup"><span data-stu-id="939dc-103">Delete groupPolicyPresentationLongDecimalTextBox</span></span>

> <span data-ttu-id="939dc-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="939dc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="939dc-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="939dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="939dc-106">[GroupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="939dc-106">Deletes a [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="939dc-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="939dc-107">Prerequisites</span></span>
<span data-ttu-id="939dc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="939dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="939dc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="939dc-110">Permission type</span></span>|<span data-ttu-id="939dc-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="939dc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="939dc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="939dc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="939dc-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="939dc-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="939dc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="939dc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="939dc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="939dc-115">Not supported.</span></span>|
|<span data-ttu-id="939dc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="939dc-116">Application</span></span>|<span data-ttu-id="939dc-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="939dc-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="939dc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="939dc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="939dc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="939dc-119">Request headers</span></span>
|<span data-ttu-id="939dc-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="939dc-120">Header</span></span>|<span data-ttu-id="939dc-121">値</span><span class="sxs-lookup"><span data-stu-id="939dc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="939dc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="939dc-122">Authorization</span></span>|<span data-ttu-id="939dc-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="939dc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="939dc-124">承諾</span><span class="sxs-lookup"><span data-stu-id="939dc-124">Accept</span></span>|<span data-ttu-id="939dc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="939dc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="939dc-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="939dc-126">Request body</span></span>
<span data-ttu-id="939dc-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="939dc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="939dc-128">応答</span><span class="sxs-lookup"><span data-stu-id="939dc-128">Response</span></span>
<span data-ttu-id="939dc-129">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="939dc-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="939dc-130">例</span><span class="sxs-lookup"><span data-stu-id="939dc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="939dc-131">要求</span><span class="sxs-lookup"><span data-stu-id="939dc-131">Request</span></span>
<span data-ttu-id="939dc-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="939dc-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="939dc-133">応答</span><span class="sxs-lookup"><span data-stu-id="939dc-133">Response</span></span>
<span data-ttu-id="939dc-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="939dc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






