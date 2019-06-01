---
title: Azure AD アクセス レビュー
description: Azure AD access レビューを使用して、ユーザーのアクセス権の構成に対して1回限りまたは定期的なアクセスレビューを構成できます。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d38d82d00c5ba83bc3b16cd05b69e99ec7c5aa2e
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34656826"
---
# <a name="azure-ad-access-reviews"></a>Azure AD アクセス レビュー

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[AZURE AD access レビュー](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview)を使用して、ユーザーのアクセス権の構成に対して1回限りまたは定期的なアクセスレビューを構成できます。

グループメンバーシップとアプリケーションアクセスのアクセスレビューに関する一般的なお客様のシナリオは、次のとおりです。
   
- お客様は、アクセスレビューを使用して、アプリケーションおよびグループのメンバーシップへのアクセスに関するレビューを使用して、ゲストユーザーのアクセスを確認し、証明できます。 レビュー担当者は、提供された洞察を使用して、ゲストのアクセスを継続する必要があるかどうかを効率的に決定できます。
      
- お客様は、アクセスレビューを使用して、アプリケーションおよびグループメンバーシップへの従業員のアクセスを確認し、証明することができます。
   
- お客様は、コンプライアンスまたはリスクに敏感なアプリケーションのレビューを追跡するために、組織が関連するプログラムにアクセスレビューコントロールを収集できます。

また、グローバル管理者または Azure サブスクリプションの役割などの Azure AD の役割に割り当てられている管理ユーザーの役割割り当てを確認し、証明するための関連機能もあります。  この機能は、 [AZURE AD Privileged Identity Management](privilegedidentitymanagement-root.md)に含まれています。

アクセスレビュー機能 (API を含む) は Azure AD Premium P2 に含まれていることに注意してください。  アクセスレビューを作成するテナントには、有効な、購入済みまたは試用版の Azure AD プレミアム P2 または EMS E5 サブスクリプションが必要です。 アクセスレビュー、プログラム、またはプログラムの制御を作成する前に、管理者は、利用を事前[](programcontroltype.md)に設定し[](businessflowtemplate.md)ておく必要があります。 Azure ad のアクセスレビューに、または azure ad の役割または azure サブスクリプションの役割のアクセスレビューの場合は azure ad PIM に、組織をオンボードにすることができます。


## <a name="methods"></a>メソッド 

次の表に、アクセスレビュー関連のリソースを操作するために使用できるメソッドを示します。

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[AccessReview を取得する](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   特定の ID を持つアクセスレビューを取得します。 |
|[AccessReview を作成する](../api/accessreview-create.md) | [accessReview](accessreview.md) |   新しい accessReview を作成します。 |
|[AccessReview の削除](../api/accessreview-delete.md) | なし。   | AccessReview を削除します。 |
|[AccessReview を更新する](../api/accessreview-update.md) | [accessReview](accessreview.md) | AccessReview を更新します。 |
|[AccessReview レビュー担当者のリスト](../api/accessreview-listreviewers.md) |      [Useridentity](useridentity.md)コレクション| AccessReview のレビュー担当者を取得します。 |
|[AccessReview レビュー担当者を追加する](../api/accessreview-addreviewer.md) |      なし。   |   閲覧者を accessReview に追加します。 |
|[AccessReview レビュー担当者を削除する](../api/accessreview-removereviewer.md) | なし。  |   AccessReview からレビュー担当者を削除します。 |
|[AccessReview に関する決定事項を一覧表示する](../api/accessreview-listdecisions.md) |      [accessReviewDecision](accessreviewdecision.md)コレクション| AccessReview の決定事項を取得します。|
|[自分の accessReview の決定事項を一覧表示する](../api/accessreview-listmydecisions.md) |     [accessReviewDecision](accessreviewdecision.md)コレクション| レビュー担当者として、accessReview の決定事項を取得します。|
|[Access レビュー通知の送信](../api/accessreview-sendreminder.md) |        なし。   |   AccessReview のレビュー担当者に通知を送信します。 |
|[AccessReview を停止する](../api/accessreview-stop.md) |     なし。   |   AccessReview を停止します。 |
|[AccessReview の決定をリセットする](../api/accessreview-reset.md) |     なし。   |   進行中の accessReview で意思決定をリセットします。|
|[AccessReview の決定を適用する](../api/accessreview-apply.md) |     なし。   |   完了した accessReview から決定を適用します。|
|[BusinessFlowTemplates を一覧表示する](../api/businessflowtemplate-list.md) | [Businessflowtemplate](businessflowtemplate.md)コレクション| レビューにアクセスするための適切なビジネスフローテンプレートを取得します。|
|[プログラムを作成する](../api/program-create.md) |   [アプリケーション](program.md)   |   新しいプログラムを作成します。|
|[プログラムの削除](../api/program-delete.md) |   なし。   |   プログラムを削除します。|
|[プログラムの一覧表示](../api/program-list.md) |  [プログラム](program.md)コレクション|   すべてのプログラムのコレクションを取得します。|
|[プログラムの programControls を一覧表示する](../api/program-listcontrols.md) |      [Programcontrol](programcontrol.md)コレクション| プログラムのコントロールのコレクションを取得します。|
|[プログラムの更新](../api/program-update.md) |   [アプリケーション](program.md)|  プログラムを更新します。|
|[ProgramControl を作成する](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   プログラムに programControl を追加します。|
|[ProgramControl の削除](../api/programcontrol-delete.md) |     なし。   |   プログラムから programControl を削除します。|
|[ProgramControls のリスト](../api/programcontrol-list.md) | [Programcontrol](programcontrol.md)コレクション| テナント内のすべてのプログラムでコントロールを一覧表示します。|
|[ProgramControlTypes のリスト](../api/programcontroltype-list.md) | [Programcontroltype](programcontroltype.md)コレクション| プログラムコントロールの種類を一覧表示します。 |

## <a name="role-and-application-permission-authorization-checks"></a>役割とアプリケーションのアクセス許可の承認チェック

呼び出し元ユーザーがアクセスレビュー、プログラム、および制御を管理するには、次のディレクトリの役割が必要です。

| ターゲットリソース | Operation | アプリケーションのアクセス許可 | 呼び出し元ユーザーの必要なディレクトリの役割 |
|:----------------|:------------------|:------------|:--------------------------------------------|
|Azure AD ロールの[Accessreview](accessreview.md) | 読み取り | AccessReview を参照してください。すべてのまたは AccessReview. | 全体管理者、セキュリティ管理者、セキュリティリーダ、または特権ロール管理者 |
|Azure AD ロールの[Accessreview](accessreview.md) | 作成、更新、または削除 | AccessReview.ReadWrite.All | グローバル管理者または特権ロール管理者 |
|グループまたはアプリの[Accessreview](accessreview.md) | 読み取り | AccessReview を参照してください。すべてのまたは AccessReview. | グローバル管理者、セキュリティ管理者、セキュリティリーダ、またはユーザー管理者 |
|グループまたはアプリの[Accessreview](accessreview.md) | 作成、更新、または削除 | AccessReview.ReadWrite.All | 全体管理者またはユーザー管理者 |
| [プログラム](program.md)および[programcontrol](programcontrol.md)| 読み取り | ProgramControl. すべてのまたはすべてのプログラムを読み取ることができます。 |  グローバル管理者、セキュリティ管理者、セキュリティリーダ、またはユーザー管理者 |
| [プログラム](program.md)および[programcontrol](programcontrol.md) | 作成、更新、または削除 | ProgramControl.ReadWrite.All | 全体管理者またはユーザー管理者 |

また、アクセスレビューの担当者に割り当てられているユーザーは、ディレクトリロールに存在しなくても、決定を管理できます。

## <a name="see-also"></a>関連項目

- [管理者が Azure AD アクセスレビューを使用してユーザーアクセスを管理する方法](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [管理者が Azure AD アクセスレビューでゲストアクセスを管理する方法](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)
- [管理者が Azure AD アクセスレビューのプログラムとコントロールを管理する方法](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-programs-controls)


<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
