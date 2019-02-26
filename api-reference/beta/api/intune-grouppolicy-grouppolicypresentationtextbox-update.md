---
title: grouppolicypresentationtextbox の更新
description: grouppolicypresentationtextbox オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f9cc29531d8318be47e1738fdc6d51dca8f044b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152137"
---
# <a name="update-grouppolicypresentationtextbox"></a><span data-ttu-id="7e2af-103">grouppolicypresentationtextbox の更新</span><span class="sxs-lookup"><span data-stu-id="7e2af-103">Update groupPolicyPresentationTextBox</span></span>

> <span data-ttu-id="7e2af-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e2af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e2af-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7e2af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e2af-106">[grouppolicypresentationtextbox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7e2af-106">Update the properties of a [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e2af-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7e2af-107">Prerequisites</span></span>
<span data-ttu-id="7e2af-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7e2af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7e2af-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7e2af-110">Permission type</span></span>|<span data-ttu-id="7e2af-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7e2af-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e2af-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7e2af-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7e2af-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e2af-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7e2af-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7e2af-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e2af-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e2af-115">Not supported.</span></span>|
|<span data-ttu-id="7e2af-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7e2af-116">Application</span></span>|<span data-ttu-id="7e2af-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e2af-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e2af-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7e2af-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="7e2af-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7e2af-119">Request headers</span></span>
|<span data-ttu-id="7e2af-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7e2af-120">Header</span></span>|<span data-ttu-id="7e2af-121">値</span><span class="sxs-lookup"><span data-stu-id="7e2af-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e2af-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e2af-122">Authorization</span></span>|<span data-ttu-id="7e2af-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7e2af-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e2af-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7e2af-124">Accept</span></span>|<span data-ttu-id="7e2af-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7e2af-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e2af-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7e2af-126">Request body</span></span>
<span data-ttu-id="7e2af-127">要求本文で、 [grouppolicypresentationtextbox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7e2af-127">In the request body, supply a JSON representation for the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

<span data-ttu-id="7e2af-128">次の表に、 [grouppolicypresentationtextbox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7e2af-128">The following table shows the properties that are required when you create the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md).</span></span>

|<span data-ttu-id="7e2af-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e2af-129">Property</span></span>|<span data-ttu-id="7e2af-130">型</span><span class="sxs-lookup"><span data-stu-id="7e2af-130">Type</span></span>|<span data-ttu-id="7e2af-131">説明</span><span class="sxs-lookup"><span data-stu-id="7e2af-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e2af-132">label</span><span class="sxs-lookup"><span data-stu-id="7e2af-132">label</span></span>|<span data-ttu-id="7e2af-133">String</span><span class="sxs-lookup"><span data-stu-id="7e2af-133">String</span></span>|<span data-ttu-id="7e2af-134">任意のプレゼンテーションエンティティのローカライズされたテキストラベル。</span><span class="sxs-lookup"><span data-stu-id="7e2af-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="7e2af-135">既定値は empty です。</span><span class="sxs-lookup"><span data-stu-id="7e2af-135">The default value is empty.</span></span> <span data-ttu-id="7e2af-136">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7e2af-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="7e2af-137">id</span><span class="sxs-lookup"><span data-stu-id="7e2af-137">id</span></span>|<span data-ttu-id="7e2af-138">String</span><span class="sxs-lookup"><span data-stu-id="7e2af-138">String</span></span>|<span data-ttu-id="7e2af-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7e2af-139">Key of the entity.</span></span> <span data-ttu-id="7e2af-140">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7e2af-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="7e2af-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7e2af-141">lastModifiedDateTime</span></span>|<span data-ttu-id="7e2af-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e2af-142">DateTimeOffset</span></span>|<span data-ttu-id="7e2af-143">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="7e2af-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="7e2af-144">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7e2af-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="7e2af-145">defaultValue</span><span class="sxs-lookup"><span data-stu-id="7e2af-145">defaultValue</span></span>|<span data-ttu-id="7e2af-146">文字列</span><span class="sxs-lookup"><span data-stu-id="7e2af-146">String</span></span>|<span data-ttu-id="7e2af-147">テキストボックスに表示されるローカライズされた既定の文字列。</span><span class="sxs-lookup"><span data-stu-id="7e2af-147">Localized default string displayed in the text box.</span></span> <span data-ttu-id="7e2af-148">既定値は empty です。</span><span class="sxs-lookup"><span data-stu-id="7e2af-148">The default value is empty.</span></span>|
|<span data-ttu-id="7e2af-149">必須</span><span class="sxs-lookup"><span data-stu-id="7e2af-149">required</span></span>|<span data-ttu-id="7e2af-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e2af-150">Boolean</span></span>|<span data-ttu-id="7e2af-151">テキストボックスに値を入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7e2af-151">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="7e2af-152">既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="7e2af-152">Default value is false.</span></span>|
|<span data-ttu-id="7e2af-153">maxLength</span><span class="sxs-lookup"><span data-stu-id="7e2af-153">maxLength</span></span>|<span data-ttu-id="7e2af-154">Int64</span><span class="sxs-lookup"><span data-stu-id="7e2af-154">Int64</span></span>|<span data-ttu-id="7e2af-155">テキストの最大文字数を指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="7e2af-155">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="7e2af-156">既定値は1023です。</span><span class="sxs-lookup"><span data-stu-id="7e2af-156">Default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="7e2af-157">応答</span><span class="sxs-lookup"><span data-stu-id="7e2af-157">Response</span></span>
<span data-ttu-id="7e2af-158">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[grouppolicypresentationtextbox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7e2af-158">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e2af-159">例</span><span class="sxs-lookup"><span data-stu-id="7e2af-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e2af-160">要求</span><span class="sxs-lookup"><span data-stu-id="7e2af-160">Request</span></span>
<span data-ttu-id="7e2af-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7e2af-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 181

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "Label value",
  "defaultValue": "Default Value value",
  "required": true,
  "maxLength": 9
}
```

### <a name="response"></a><span data-ttu-id="7e2af-162">応答</span><span class="sxs-lookup"><span data-stu-id="7e2af-162">Response</span></span>
<span data-ttu-id="7e2af-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7e2af-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 294

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "Label value",
  "id": "ec80633e-633e-ec80-3e63-80ec3e6380ec",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": "Default Value value",
  "required": true,
  "maxLength": 9
}
```




