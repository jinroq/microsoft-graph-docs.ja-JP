---
title: groupPolicyPresentation の更新
description: groupPolicyPresentation オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 44da489c3cdf124b434ba35d52d39d63dba54209
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986979"
---
# <a name="update-grouppolicypresentation"></a><span data-ttu-id="3ce30-103">groupPolicyPresentation の更新</span><span class="sxs-lookup"><span data-stu-id="3ce30-103">Update groupPolicyPresentation</span></span>

> <span data-ttu-id="3ce30-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ce30-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ce30-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3ce30-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ce30-106">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3ce30-106">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ce30-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="3ce30-107">Prerequisites</span></span>
<span data-ttu-id="3ce30-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3ce30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ce30-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3ce30-110">Permission type</span></span>|<span data-ttu-id="3ce30-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3ce30-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ce30-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3ce30-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3ce30-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ce30-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3ce30-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3ce30-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ce30-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ce30-115">Not supported.</span></span>|
|<span data-ttu-id="3ce30-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3ce30-116">Application</span></span>|<span data-ttu-id="3ce30-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ce30-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ce30-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3ce30-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="3ce30-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3ce30-119">Request headers</span></span>
|<span data-ttu-id="3ce30-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3ce30-120">Header</span></span>|<span data-ttu-id="3ce30-121">値</span><span class="sxs-lookup"><span data-stu-id="3ce30-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ce30-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ce30-122">Authorization</span></span>|<span data-ttu-id="3ce30-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="3ce30-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ce30-124">承諾</span><span class="sxs-lookup"><span data-stu-id="3ce30-124">Accept</span></span>|<span data-ttu-id="3ce30-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3ce30-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ce30-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3ce30-126">Request body</span></span>
<span data-ttu-id="3ce30-127">要求本文で、 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3ce30-127">In the request body, supply a JSON representation for the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

<span data-ttu-id="3ce30-128">次の表に、 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3ce30-128">The following table shows the properties that are required when you create the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md).</span></span>

|<span data-ttu-id="3ce30-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ce30-129">Property</span></span>|<span data-ttu-id="3ce30-130">型</span><span class="sxs-lookup"><span data-stu-id="3ce30-130">Type</span></span>|<span data-ttu-id="3ce30-131">説明</span><span class="sxs-lookup"><span data-stu-id="3ce30-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ce30-132">label</span><span class="sxs-lookup"><span data-stu-id="3ce30-132">label</span></span>|<span data-ttu-id="3ce30-133">String</span><span class="sxs-lookup"><span data-stu-id="3ce30-133">String</span></span>|<span data-ttu-id="3ce30-134">任意のプレゼンテーションエンティティのローカライズされたテキストラベル。</span><span class="sxs-lookup"><span data-stu-id="3ce30-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="3ce30-135">既定値は空白です。</span><span class="sxs-lookup"><span data-stu-id="3ce30-135">The default value is empty.</span></span>|
|<span data-ttu-id="3ce30-136">id</span><span class="sxs-lookup"><span data-stu-id="3ce30-136">id</span></span>|<span data-ttu-id="3ce30-137">String</span><span class="sxs-lookup"><span data-stu-id="3ce30-137">String</span></span>|<span data-ttu-id="3ce30-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3ce30-138">Key of the entity.</span></span>|
|<span data-ttu-id="3ce30-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ce30-139">lastModifiedDateTime</span></span>|<span data-ttu-id="3ce30-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ce30-140">DateTimeOffset</span></span>|<span data-ttu-id="3ce30-141">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="3ce30-141">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="3ce30-142">応答</span><span class="sxs-lookup"><span data-stu-id="3ce30-142">Response</span></span>
<span data-ttu-id="3ce30-143">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3ce30-143">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ce30-144">例</span><span class="sxs-lookup"><span data-stu-id="3ce30-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ce30-145">要求</span><span class="sxs-lookup"><span data-stu-id="3ce30-145">Request</span></span>
<span data-ttu-id="3ce30-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3ce30-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="3ce30-147">応答</span><span class="sxs-lookup"><span data-stu-id="3ce30-147">Response</span></span>
<span data-ttu-id="3ce30-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3ce30-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 205

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "Label value",
  "id": "a33caa6a-aa6a-a33c-6aaa-3ca36aaa3ca3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




