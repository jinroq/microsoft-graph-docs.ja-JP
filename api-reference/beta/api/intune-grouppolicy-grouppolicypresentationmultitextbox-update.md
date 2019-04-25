---
title: grouppolicypresentationmultitextbox の更新
description: grouppolicypresentationmultitextbox オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b2aa9e5005269d2385f807f3eac9d16388e70cae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32530908"
---
# <a name="update-grouppolicypresentationmultitextbox"></a><span data-ttu-id="f3a95-103">grouppolicypresentationmultitextbox の更新</span><span class="sxs-lookup"><span data-stu-id="f3a95-103">Update groupPolicyPresentationMultiTextBox</span></span>

> <span data-ttu-id="f3a95-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3a95-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3a95-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3a95-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3a95-106">[grouppolicypresentationmultitextbox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f3a95-106">Update the properties of a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3a95-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f3a95-107">Prerequisites</span></span>
<span data-ttu-id="f3a95-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3a95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3a95-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f3a95-110">Permission type</span></span>|<span data-ttu-id="f3a95-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f3a95-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3a95-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f3a95-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3a95-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3a95-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f3a95-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f3a95-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3a95-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3a95-115">Not supported.</span></span>|
|<span data-ttu-id="f3a95-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f3a95-116">Application</span></span>|<span data-ttu-id="f3a95-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3a95-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3a95-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f3a95-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="f3a95-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3a95-119">Request headers</span></span>
|<span data-ttu-id="f3a95-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3a95-120">Header</span></span>|<span data-ttu-id="f3a95-121">値</span><span class="sxs-lookup"><span data-stu-id="f3a95-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3a95-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3a95-122">Authorization</span></span>|<span data-ttu-id="f3a95-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3a95-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3a95-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f3a95-124">Accept</span></span>|<span data-ttu-id="f3a95-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f3a95-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3a95-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f3a95-126">Request body</span></span>
<span data-ttu-id="f3a95-127">要求本文で、 [grouppolicypresentationmultitextbox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f3a95-127">In the request body, supply a JSON representation for the [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

<span data-ttu-id="f3a95-128">次の表に、 [grouppolicypresentationmultitextbox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f3a95-128">The following table shows the properties that are required when you create the [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md).</span></span>

|<span data-ttu-id="f3a95-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3a95-129">Property</span></span>|<span data-ttu-id="f3a95-130">型</span><span class="sxs-lookup"><span data-stu-id="f3a95-130">Type</span></span>|<span data-ttu-id="f3a95-131">説明</span><span class="sxs-lookup"><span data-stu-id="f3a95-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3a95-132">label</span><span class="sxs-lookup"><span data-stu-id="f3a95-132">label</span></span>|<span data-ttu-id="f3a95-133">String</span><span class="sxs-lookup"><span data-stu-id="f3a95-133">String</span></span>|<span data-ttu-id="f3a95-134">任意のプレゼンテーションエンティティのローカライズされたテキストラベル。</span><span class="sxs-lookup"><span data-stu-id="f3a95-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="f3a95-135">既定値は空白です。</span><span class="sxs-lookup"><span data-stu-id="f3a95-135">The default value is empty.</span></span> <span data-ttu-id="f3a95-136">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f3a95-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="f3a95-137">id</span><span class="sxs-lookup"><span data-stu-id="f3a95-137">id</span></span>|<span data-ttu-id="f3a95-138">String</span><span class="sxs-lookup"><span data-stu-id="f3a95-138">String</span></span>|<span data-ttu-id="f3a95-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f3a95-139">Key of the entity.</span></span> <span data-ttu-id="f3a95-140">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f3a95-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="f3a95-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3a95-141">lastModifiedDateTime</span></span>|<span data-ttu-id="f3a95-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3a95-142">DateTimeOffset</span></span>|<span data-ttu-id="f3a95-143">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="f3a95-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="f3a95-144">[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f3a95-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="f3a95-145">必須</span><span class="sxs-lookup"><span data-stu-id="f3a95-145">required</span></span>|<span data-ttu-id="f3a95-146">ブール値</span><span class="sxs-lookup"><span data-stu-id="f3a95-146">Boolean</span></span>|<span data-ttu-id="f3a95-147">テキストボックスに値を入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f3a95-147">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="f3a95-148">既定値は False です。</span><span class="sxs-lookup"><span data-stu-id="f3a95-148">Default value is false.</span></span>|
|<span data-ttu-id="f3a95-149">maxLength</span><span class="sxs-lookup"><span data-stu-id="f3a95-149">maxLength</span></span>|<span data-ttu-id="f3a95-150">Int64</span><span class="sxs-lookup"><span data-stu-id="f3a95-150">Int64</span></span>|<span data-ttu-id="f3a95-151">テキストの最大文字数を指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="f3a95-151">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="f3a95-152">既定値は1023です。</span><span class="sxs-lookup"><span data-stu-id="f3a95-152">Default value is 1023.</span></span>|
|<span data-ttu-id="f3a95-153">maxstrings</span><span class="sxs-lookup"><span data-stu-id="f3a95-153">maxStrings</span></span>|<span data-ttu-id="f3a95-154">Int64</span><span class="sxs-lookup"><span data-stu-id="f3a95-154">Int64</span></span>|<span data-ttu-id="f3a95-155">文字列の最大数を指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="f3a95-155">An unsigned integer that specifies the maximum number of strings.</span></span> <span data-ttu-id="f3a95-156">既定値は 0 です。</span><span class="sxs-lookup"><span data-stu-id="f3a95-156">Default value is 0.</span></span>|



## <a name="response"></a><span data-ttu-id="f3a95-157">応答</span><span class="sxs-lookup"><span data-stu-id="f3a95-157">Response</span></span>
<span data-ttu-id="f3a95-158">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[grouppolicypresentationmultitextbox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f3a95-158">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3a95-159">例</span><span class="sxs-lookup"><span data-stu-id="f3a95-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3a95-160">要求</span><span class="sxs-lookup"><span data-stu-id="f3a95-160">Request</span></span>
<span data-ttu-id="f3a95-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f3a95-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
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

### <a name="response"></a><span data-ttu-id="f3a95-162">応答</span><span class="sxs-lookup"><span data-stu-id="f3a95-162">Response</span></span>
<span data-ttu-id="f3a95-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f3a95-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





