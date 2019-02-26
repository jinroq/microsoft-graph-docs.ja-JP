---
title: grouppolicypresentationmultitextbox の作成
description: 新しい grouppolicypresentationmultitextbox オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bdde2677c4852c70f1693e7a16e2b9e3fb048388
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152102"
---
# <a name="create-grouppolicypresentationmultitextbox"></a><span data-ttu-id="97008-103">grouppolicypresentationmultitextbox の作成</span><span class="sxs-lookup"><span data-stu-id="97008-103">Create groupPolicyPresentationMultiTextBox</span></span>

> <span data-ttu-id="97008-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97008-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97008-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="97008-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97008-106">新しい[grouppolicypresentationmultitextbox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="97008-106">Create a new [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97008-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="97008-107">Prerequisites</span></span>
<span data-ttu-id="97008-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="97008-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="97008-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="97008-110">Permission type</span></span>|<span data-ttu-id="97008-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="97008-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97008-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="97008-112">Delegated (work or school account)</span></span>|<span data-ttu-id="97008-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97008-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="97008-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="97008-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97008-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97008-115">Not supported.</span></span>|
|<span data-ttu-id="97008-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="97008-116">Application</span></span>|<span data-ttu-id="97008-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97008-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97008-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="97008-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="97008-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="97008-119">Request headers</span></span>
|<span data-ttu-id="97008-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="97008-120">Header</span></span>|<span data-ttu-id="97008-121">値</span><span class="sxs-lookup"><span data-stu-id="97008-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97008-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="97008-122">Authorization</span></span>|<span data-ttu-id="97008-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="97008-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97008-124">承諾</span><span class="sxs-lookup"><span data-stu-id="97008-124">Accept</span></span>|<span data-ttu-id="97008-125">application/json</span><span class="sxs-lookup"><span data-stu-id="97008-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97008-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="97008-126">Request body</span></span>
<span data-ttu-id="97008-127">要求本文で、grouppolicypresentationmultitextbox オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="97008-127">In the request body, supply a JSON representation for the groupPolicyPresentationMultiTextBox object.</span></span>

<span data-ttu-id="97008-128">次の表に、grouppolicypresentationmultitextbox の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="97008-128">The following table shows the properties that are required when you create the groupPolicyPresentationMultiTextBox.</span></span>

|<span data-ttu-id="97008-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97008-129">Property</span></span>|<span data-ttu-id="97008-130">型</span><span class="sxs-lookup"><span data-stu-id="97008-130">Type</span></span>|<span data-ttu-id="97008-131">説明</span><span class="sxs-lookup"><span data-stu-id="97008-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97008-132">label</span><span class="sxs-lookup"><span data-stu-id="97008-132">label</span></span>|<span data-ttu-id="97008-133">String</span><span class="sxs-lookup"><span data-stu-id="97008-133">String</span></span>|<span data-ttu-id="97008-134">任意のプレゼンテーションエンティティのローカライズされたテキストラベル。</span><span class="sxs-lookup"><span data-stu-id="97008-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="97008-135">既定値は empty です。</span><span class="sxs-lookup"><span data-stu-id="97008-135">The default value is empty.</span></span> <span data-ttu-id="97008-136">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="97008-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="97008-137">id</span><span class="sxs-lookup"><span data-stu-id="97008-137">id</span></span>|<span data-ttu-id="97008-138">String</span><span class="sxs-lookup"><span data-stu-id="97008-138">String</span></span>|<span data-ttu-id="97008-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="97008-139">Key of the entity.</span></span> <span data-ttu-id="97008-140">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="97008-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="97008-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97008-141">lastModifiedDateTime</span></span>|<span data-ttu-id="97008-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97008-142">DateTimeOffset</span></span>|<span data-ttu-id="97008-143">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="97008-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="97008-144">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="97008-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="97008-145">必須</span><span class="sxs-lookup"><span data-stu-id="97008-145">required</span></span>|<span data-ttu-id="97008-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="97008-146">Boolean</span></span>|<span data-ttu-id="97008-147">テキストボックスに値を入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="97008-147">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="97008-148">既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="97008-148">Default value is false.</span></span>|
|<span data-ttu-id="97008-149">maxLength</span><span class="sxs-lookup"><span data-stu-id="97008-149">maxLength</span></span>|<span data-ttu-id="97008-150">Int64</span><span class="sxs-lookup"><span data-stu-id="97008-150">Int64</span></span>|<span data-ttu-id="97008-151">テキストの最大文字数を指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="97008-151">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="97008-152">既定値は1023です。</span><span class="sxs-lookup"><span data-stu-id="97008-152">Default value is 1023.</span></span>|
|<span data-ttu-id="97008-153">maxstrings</span><span class="sxs-lookup"><span data-stu-id="97008-153">maxStrings</span></span>|<span data-ttu-id="97008-154">Int64</span><span class="sxs-lookup"><span data-stu-id="97008-154">Int64</span></span>|<span data-ttu-id="97008-155">文字列の最大数を指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="97008-155">An unsigned integer that specifies the maximum number of strings.</span></span> <span data-ttu-id="97008-156">既定値は0です。</span><span class="sxs-lookup"><span data-stu-id="97008-156">Default value is 0.</span></span>|



## <a name="response"></a><span data-ttu-id="97008-157">応答</span><span class="sxs-lookup"><span data-stu-id="97008-157">Response</span></span>
<span data-ttu-id="97008-158">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[grouppolicypresentationmultitextbox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="97008-158">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97008-159">例</span><span class="sxs-lookup"><span data-stu-id="97008-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="97008-160">要求</span><span class="sxs-lookup"><span data-stu-id="97008-160">Request</span></span>
<span data-ttu-id="97008-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="97008-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 165

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "label": "Label value",
  "required": true,
  "maxLength": 9,
  "maxStrings": 10
}
```

### <a name="response"></a><span data-ttu-id="97008-162">応答</span><span class="sxs-lookup"><span data-stu-id="97008-162">Response</span></span>
<span data-ttu-id="97008-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="97008-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 278

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "label": "Label value",
  "id": "381ac035-c035-381a-35c0-1a3835c01a38",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "required": true,
  "maxLength": 9,
  "maxStrings": 10
}
```




