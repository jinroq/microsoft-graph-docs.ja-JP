---
title: GroupPolicyPresentationText を削除します。
description: GroupPolicyPresentationText を削除します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5e4872fbf4cd124b1637f893bda3685b414c4178
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430314"
---
# <a name="delete-grouppolicypresentationtext"></a><span data-ttu-id="9f417-103">GroupPolicyPresentationText を削除します。</span><span class="sxs-lookup"><span data-stu-id="9f417-103">Delete groupPolicyPresentationText</span></span>

> <span data-ttu-id="9f417-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9f417-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9f417-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f417-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f417-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9f417-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f417-107">の[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="9f417-107">Deletes a [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f417-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9f417-108">Prerequisites</span></span>
<span data-ttu-id="9f417-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9f417-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9f417-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9f417-111">Permission type</span></span>|<span data-ttu-id="9f417-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9f417-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f417-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9f417-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f417-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f417-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9f417-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9f417-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f417-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f417-116">Not supported.</span></span>|
|<span data-ttu-id="9f417-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9f417-117">Application</span></span>|<span data-ttu-id="9f417-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f417-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f417-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9f417-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="9f417-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9f417-120">Request headers</span></span>
|<span data-ttu-id="9f417-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9f417-121">Header</span></span>|<span data-ttu-id="9f417-122">値</span><span class="sxs-lookup"><span data-stu-id="9f417-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f417-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f417-123">Authorization</span></span>|<span data-ttu-id="9f417-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9f417-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f417-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9f417-125">Accept</span></span>|<span data-ttu-id="9f417-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9f417-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f417-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9f417-127">Request body</span></span>
<span data-ttu-id="9f417-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9f417-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f417-129">応答</span><span class="sxs-lookup"><span data-stu-id="9f417-129">Response</span></span>
<span data-ttu-id="9f417-130">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="9f417-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9f417-131">例</span><span class="sxs-lookup"><span data-stu-id="9f417-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f417-132">要求</span><span class="sxs-lookup"><span data-stu-id="9f417-132">Request</span></span>
<span data-ttu-id="9f417-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9f417-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="9f417-134">応答</span><span class="sxs-lookup"><span data-stu-id="9f417-134">Response</span></span>
<span data-ttu-id="9f417-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9f417-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




